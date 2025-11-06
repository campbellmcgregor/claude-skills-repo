# Typography Reference

## Font Fundamentals

### Font Classifications

**Serif** - Traditional, formal, readable in print  
Examples: Georgia, Times New Roman, Merriweather  
Best for: Long-form content, traditional brands

**Sans-Serif** - Modern, clean, readable on screens  
Examples: Helvetica, Arial, Inter, Roboto  
Best for: UI, headings, digital content

**Monospace** - Fixed-width, technical  
Examples: Courier, Monaco, Fira Code  
Best for: Code blocks, data tables

**Display** - Decorative, attention-grabbing  
Examples: Playfair, Bebas Neue  
Best for: Headlines only, used sparingly

### Font Anatomy
- **x-height** - Height of lowercase letters (affects readability)
- **Ascender** - Part above x-height (b, d, h)
- **Descender** - Part below baseline (g, p, q)
- **Kerning** - Space between letter pairs
- **Tracking** - Overall letter spacing

## Type Scale

### Modular Scale System
Base size: 16px  
Scale ratio: 1.25 (Major Third)

```
12px (0.75rem) - xs - Fine print, captions
14px (0.875rem) - sm - Secondary text, labels
16px (1rem) - base - Body text
20px (1.25rem) - lg - Lead paragraph
24px (1.5rem) - xl - Small headings
30px (1.875rem) - 2xl - H3
36px (2.25rem) - 3xl - H2
48px (3rem) - 4xl - H1
60px (3.75rem) - 5xl - Display
72px (4.5rem) - 6xl - Hero
```

### Responsive Typography
```css
/* Mobile: smaller scale */
h1 { font-size: 2rem; }    /* 32px */
h2 { font-size: 1.5rem; }  /* 24px */
body { font-size: 1rem; }   /* 16px */

/* Desktop: larger scale */
@media (min-width: 768px) {
  h1 { font-size: 3rem; }    /* 48px */
  h2 { font-size: 2.25rem; } /* 36px */
  body { font-size: 1rem; }   /* 16px stays same */
}
```

## Font Pairing

### Classic Combinations

**Serif + Sans-Serif** (most common)  
- Merriweather (headings) + Open Sans (body)
- Playfair Display (headings) + Source Sans Pro (body)
- Lora (headings) + Roboto (body)

**Sans + Sans** (modern, minimal)  
- Montserrat (headings) + Lato (body)
- Poppins (headings) + Inter (body)
- Work Sans (headings) + IBM Plex Sans (body)

**Display + Sans** (creative, bold)  
- Bebas Neue (headlines) + Roboto (body)
- Oswald (headings) + Raleway (body)

### Pairing Rules
1. **Contrast** - Different enough to distinguish roles
2. **Complement** - Share similar mood/era
3. **Limit fonts** - Max 2-3 fonts per project
4. **Hierarchy** - One font for headings, one for body
5. **Test readability** - Always check body text at size

## Font Weights

### Common Weights
- **100-300 (Thin/Light)** - Large headings, decorative
- **400 (Regular)** - Body text, default
- **500-600 (Medium/Semibold)** - Emphasis, buttons
- **700 (Bold)** - Headings, strong emphasis
- **800-900 (Extrabold/Black)** - Display, hero text

### Usage Guidelines
```
Body text: 400 (regular)
Strong emphasis: 600 or 700 (semibold/bold)
Buttons: 500 or 600 (medium/semibold)
H1-H3: 700 (bold)
Fine print: 400 (regular, smaller size instead of lighter weight)
```

## Line Height (Leading)

### Optimal Line Heights
- **Body text (16px):** 1.5-1.6 (24-26px)
- **Large text (20px+):** 1.4-1.5
- **Headings:** 1.1-1.3 (tighter)
- **Small text (12-14px):** 1.5-1.7 (more breathing room)

### Formula
Smaller text = higher line height ratio  
Larger text = lower line height ratio

```css
body { line-height: 1.6; }
h1 { line-height: 1.2; }
small { line-height: 1.7; }
```

## Letter Spacing (Tracking)

### Guidelines
- **Body text:** 0 (default) or slight positive (0.01em)
- **Headings:** Slightly negative (-0.02em) for large sizes
- **ALL CAPS:** Increase spacing (+0.05em to +0.1em)
- **Small text:** Increase slightly (+0.01em)

```css
h1 { letter-spacing: -0.02em; }
.uppercase { letter-spacing: 0.1em; }
body { letter-spacing: 0; }
```

## Line Length

### Optimal Reading
- **Ideal:** 50-75 characters per line
- **Minimum:** 45 characters
- **Maximum:** 90 characters

```css
.prose {
  max-width: 65ch; /* 65 characters */
}

/* Or in pixels */
.article {
  max-width: 680px; /* ~60-70 chars at 16px */
}
```

## Text Hierarchy

### Establishing Hierarchy
1. **Size** - Larger = more important
2. **Weight** - Bolder = more emphasis
3. **Color** - Darker = primary, lighter = secondary
4. **Spacing** - More space = new section

### Example Hierarchy
```
H1: 48px, Bold (700), Grey-900, mb-6
H2: 36px, Bold (700), Grey-900, mb-4
H3: 24px, Semibold (600), Grey-800, mb-3
Body: 16px, Regular (400), Grey-700, mb-4
Caption: 14px, Regular (400), Grey-500, mb-2
```

## Readability Best Practices

### Body Text
- **Size:** 16px minimum (18px preferred)
- **Line height:** 1.5-1.6
- **Line length:** 50-75 characters
- **Color:** Dark grey, not pure black (#374151 vs #000000)
- **Alignment:** Left-aligned (easier to scan)

### Headings
- Clear size distinction between levels
- Adequate spacing before and after
- Shorter line lengths (30-40 characters)
- Darker color than body text

### Small Text
- **Minimum:** 12px (avoid smaller)
- **Increase line height:** 1.6-1.7
- **Medium weight:** 500 if too thin
- **Higher contrast:** Darker color

## Web Fonts

### Google Fonts (Free)
Popular choices:
- **Inter** - Modern, versatile UI font
- **Roboto** - Clean, neutral, widely used
- **Open Sans** - Friendly, readable
- **Lato** - Professional, geometric
- **Montserrat** - Bold headings
- **Merriweather** - Readable serif

### Font Loading
```css
/* Preload critical fonts */
<link rel="preload" href="font.woff2" as="font" crossorigin>

/* Display swap for performance */
@font-face {
  font-family: 'Inter';
  font-display: swap; /* Show fallback while loading */
  src: url('inter.woff2') format('woff2');
}
```

### Fallback Stack
```css
body {
  font-family: 
    'Inter',           /* Primary */
    -apple-system,     /* iOS */
    BlinkMacSystemFont, /* Chrome */
    'Segoe UI',        /* Windows */
    Roboto,            /* Android */
    sans-serif;        /* Final fallback */
}
```

## Responsive Typography

### Fluid Typography
Scale smoothly between breakpoints:

```css
/* Clamp: min, preferred (viewport-based), max */
h1 {
  font-size: clamp(2rem, 5vw, 4rem);
  /* 32px min, 5% of viewport, 64px max */
}
```

### Breakpoint-Based
```css
body {
  font-size: 16px; /* Mobile base */
}

@media (min-width: 768px) {
  body {
    font-size: 18px; /* Desktop bump */
  }
}
```

## Text Colors

### Color Hierarchy
**Primary text** (Grey-900): Main content, headings  
**Secondary text** (Grey-600): Supporting info, labels  
**Tertiary text** (Grey-500): Metadata, captions  
**Disabled text** (Grey-400): Inactive states

### Contrast Requirements
- Body text on white: 4.5:1 minimum (Grey-700 or darker)
- Large text on white: 3:1 minimum (Grey-600 works)
- White text: Use on dark backgrounds only (Grey-800+)

## Special Cases

### Links
```css
a {
  color: #3B82F6; /* Blue-500 */
  text-decoration: underline;
}

a:hover {
  color: #2563EB; /* Blue-600 */
}

/* Or underline on hover only */
a {
  text-decoration: none;
}

a:hover {
  text-decoration: underline;
}
```

### Code Snippets
```css
code {
  font-family: 'Fira Code', monospace;
  font-size: 0.875em; /* Slightly smaller */
  background: #F3F4F6; /* Light grey */
  padding: 2px 6px;
  border-radius: 3px;
  color: #E11D48; /* Red for contrast */
}
```

### ALL CAPS
```css
.caps {
  text-transform: uppercase;
  letter-spacing: 0.1em; /* Critical! */
  font-size: 0.875rem; /* Slightly smaller */
}
```

### Numbers & Data
```css
.numeric {
  font-feature-settings: 'tnum'; /* Tabular nums */
  font-variant-numeric: tabular-nums;
}
```

## Accessibility

### Key Principles
- **Minimum size:** 16px for body text
- **Minimum contrast:** 4.5:1 for normal text, 3:1 for large
- **Avoid pure black:** #374151 easier on eyes than #000000
- **Line height:** Adequate spacing for readability
- **Avoid justified text:** Creates uneven spacing

### Text Resizing
Design should work up to 200% zoom:
```css
/* Use relative units */
body { font-size: 1rem; } /* ✅ Scales */
h1 { font-size: 3rem; }   /* ✅ Scales */

/* Avoid */
p { font-size: 16px; } /* ❌ Fixed size */
```

## Common Typography Mistakes

1. **Too many fonts** - Stick to 2-3 maximum
2. **Too small body text** - 16px minimum
3. **Poor contrast** - Test with accessibility tools
4. **No hierarchy** - Size/weight variations needed
5. **Cramped line height** - 1.5+ for readability
6. **Long lines** - 50-75 characters ideal
7. **Overuse of bold** - Use sparingly for emphasis
8. **Centered body text** - Left-align for easier reading
9. **Too tight letter spacing** - Especially in ALL CAPS
10. **Pure black text** - Use dark grey instead (#374151)
