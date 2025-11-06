# Color Theory Reference

## Color Fundamentals

### Primary Properties
- **Hue** - The color itself (red, blue, yellow)
- **Saturation** - Intensity/purity of color
- **Lightness/Value** - How light or dark the color is

### Color Wheel Relationships

**Complementary** - Opposite colors (high contrast)  
Example: Blue (#0066CC) + Orange (#FF9933)

**Analogous** - Adjacent colors (harmonious)  
Example: Blue (#0066CC) + Blue-Green (#00AA88) + Green (#00CC66)

**Triadic** - Three evenly spaced colors (vibrant, balanced)  
Example: Red (#CC0033) + Yellow (#FFCC00) + Blue (#0066CC)

**Split-Complementary** - Base + two adjacent to complement  
Example: Blue (#0066CC) + Yellow-Orange (#FFAA33) + Red-Orange (#FF6633)

**Monochromatic** - One hue, varying saturation/lightness  
Example: Blue spectrum (#E6F2FF → #0066CC → #003366)

## Building a UI Color Palette

### Essential Colors

**Primary** - Brand color, main actions  
**Secondary** - Supporting brand color  
**Neutral** - Greys for text, backgrounds, borders  
**Semantic** - Success, warning, error, info

### Palette Structure

For each color, create 9 shades (50-900):
```
50  - Lightest (backgrounds)
100 - Very light (hover states)
200 - Light (borders)
300 - Light-medium
400 - Medium-light
500 - Base color (primary usage)
600 - Medium-dark
700 - Dark (hover states)
800 - Very dark (text)
900 - Darkest (emphasis)
```

### Example Palette (Blue Primary)
```
Blue-50:  #EFF6FF
Blue-100: #DBEAFE
Blue-200: #BFDBFE
Blue-300: #93C5FD
Blue-400: #60A5FA
Blue-500: #3B82F6 ← Base
Blue-600: #2563EB
Blue-700: #1D4ED8
Blue-800: #1E40AF
Blue-900: #1E3A8A
```

## Color Psychology

**Red** - Energy, urgency, passion (errors, sales)  
**Orange** - Friendly, confident, cheerful (CTAs, warnings)  
**Yellow** - Optimistic, clarity, warmth (highlights, caution)  
**Green** - Growth, success, calm (success states, eco)  
**Blue** - Trust, stability, professional (corporate, tech)  
**Purple** - Luxury, creative, wise (premium, beauty)  
**Pink** - Playful, youthful, feminine (lifestyle, social)  
**Brown** - Reliable, natural, rustic (craft, organic)  
**Black** - Sophisticated, powerful, modern (luxury, tech)  
**White** - Clean, simple, honest (minimal, medical)

## Semantic Color Usage

### Success (Green)
- Light: #D1FAE5 (background)
- Medium: #10B981 (icon/border)
- Dark: #065F46 (text)

### Warning (Yellow/Orange)
- Light: #FEF3C7 (background)
- Medium: #F59E0B (icon/border)
- Dark: #92400E (text)

### Error (Red)
- Light: #FEE2E2 (background)
- Medium: #EF4444 (icon/border)
- Dark: #991B1B (text)

### Info (Blue)
- Light: #DBEAFE (background)
- Medium: #3B82F6 (icon/border)
- Dark: #1E3A8A (text)

## Accessibility Guidelines

### Contrast Ratios (WCAG)
- **AAA** - 7:1 (ideal)
- **AA** - 4.5:1 (minimum for normal text)
- **AA Large** - 3:1 (18px+ regular, 14px+ bold)

### Testing Contrast
```
White (#FFFFFF) on Blue (#3B82F6) = 4.2:1 ⚠️ Fails AA
White (#FFFFFF) on Blue (#1E40AF) = 7.3:1 ✅ Passes AAA
```

### Color Blindness Considerations
- Don't rely on color alone (use icons + text)
- Test with protanopia/deuteranopia simulators
- Avoid red-green only indicators
- Use patterns in addition to colors

## Neutral Colors (Greys)

### Grey Scale
Essential for text, borders, backgrounds:
```
Grey-50:  #F9FAFB - Page background
Grey-100: #F3F4F6 - Card background
Grey-200: #E5E7EB - Border light
Grey-300: #D1D5DB - Border default
Grey-400: #9CA3AF - Disabled text
Grey-500: #6B7280 - Secondary text
Grey-600: #4B5563 - Primary text light
Grey-700: #374151 - Primary text
Grey-800: #1F2937 - Emphasis
Grey-900: #111827 - Headings
```

### True Black vs Grey-900
- **True Black (#000000)** - High contrast, harsh on screens
- **Grey-900 (#111827)** - Softer, easier on eyes (preferred)

## Color Combinations

### Light Mode Defaults
- **Background:** White or Grey-50
- **Surface:** White with shadow or Grey-100
- **Primary text:** Grey-900
- **Secondary text:** Grey-600
- **Border:** Grey-200 or Grey-300

### Dark Mode Defaults
- **Background:** Grey-900 or #0F1419
- **Surface:** Grey-800
- **Primary text:** Grey-50
- **Secondary text:** Grey-400
- **Border:** Grey-700

## Brand Color Selection

### Process
1. **Research competitors** - Differentiate
2. **Consider industry** - Finance = blue/green, Creative = vibrant
3. **Test across contexts** - Digital and print
4. **Create accessible palette** - Test all combinations
5. **Document usage rules** - When to use each shade

### Common Mistakes
- Too many brand colors (stick to 2-3)
- Poor contrast with white/black
- Colors too similar to each other
- Ignoring cultural color meanings

## Advanced Techniques

### Color Temperature
- **Warm** - Reds, oranges, yellows (energetic, inviting)
- **Cool** - Blues, greens, purples (calm, professional)

### Gradient Usage
```
Linear gradient (blue to purple):
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);

Subtle gradient (for depth):
background: linear-gradient(180deg, #ffffff 0%, #f8f9fa 100%);
```

### Opacity for Layering
Instead of lightening colors, use opacity:
- Primary-500 at 10% for subtle backgrounds
- Primary-500 at 20% for hover states
- Primary-500 at 100% for solid elements

### Color Modifiers in Code
```css
/* Tailwind approach */
.bg-blue-500/10  /* Blue-500 at 10% opacity */
.text-blue-600/80 /* Blue-600 at 80% opacity */
```

## Tools & Resources

### Color Generators
- Coolors.co - Palette generator
- Adobe Color - Color wheel tool
- Paletton - Scheme designer

### Accessibility Checkers
- WebAIM Contrast Checker
- Stark - Plugin for Figma/Sketch
- Who Can Use - Simulation tool

### Inspiration
- Dribbble - Design showcases
- Behance - Creative portfolios
- Brand style guides - Real-world examples
