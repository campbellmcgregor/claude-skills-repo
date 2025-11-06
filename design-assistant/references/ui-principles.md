# UI/UX Principles Reference

## Layout Fundamentals

### Spacing System
Use consistent spacing based on 4px or 8px grid:
- 4px (xs) - Tight spacing within components
- 8px (sm) - Default spacing between related elements
- 16px (md) - Spacing between component groups
- 24px (lg) - Section spacing
- 32px (xl) - Major section breaks
- 48px+ (2xl) - Page-level spacing

### Visual Hierarchy
1. **Size** - Larger = more important
2. **Weight** - Bold = emphasis
3. **Color** - Brighter/saturated = attention
4. **Position** - Top-left = primary focus (LTR languages)
5. **Whitespace** - Isolation = importance

### Layout Patterns

**F-Pattern** - Users scan top-left first (headers, nav)  
**Z-Pattern** - Eye moves diagonally (landing pages)  
**Grid System** - 12-column for flexibility  
**Card Layout** - Contained, scannable content blocks

## Component Design

### Buttons
**Primary** - Most important action (filled, high contrast)  
**Secondary** - Alternative actions (outlined or ghost)  
**Tertiary** - Subtle actions (text only)

Minimum touch target: 44x44px (mobile), 32x32px (desktop)

### Forms
- Label above input (better mobile UX)
- Clear placeholder text (light grey)
- Validation feedback (inline, immediate)
- Error states (red border + message)
- Success states (green checkmark)

### Navigation
- Primary nav: 5-7 items max
- Clear active state
- Breadcrumbs for deep hierarchies
- Consistent placement (top or left sidebar)

## Interaction Patterns

### States
Every interactive element needs:
- **Default** - Resting state
- **Hover** - Visual feedback (pointer cursor)
- **Active** - Click/press state
- **Focus** - Keyboard navigation (outline)
- **Disabled** - Reduced opacity, no interaction

### Feedback
- **Loading** - Spinner or skeleton screen
- **Success** - Checkmark, green toast
- **Error** - Clear message, red indicator
- **Empty State** - Helpful illustration + CTA

### Animations
Keep subtle:
- Transitions: 200-300ms
- Hover effects: 150ms
- Page transitions: 400ms max
- Easing: ease-in-out (natural feel)

## Accessibility

### Contrast
- Normal text: 4.5:1 minimum
- Large text (18px+): 3:1 minimum
- UI components: 3:1 minimum

### Keyboard Navigation
- Tab order follows visual order
- All interactive elements focusable
- Clear focus indicators
- Escape key closes modals

### Screen Readers
- Semantic HTML (header, nav, main, footer)
- Alt text for images
- ARIA labels for custom components
- Skip to content link

## Responsive Design

### Breakpoints
- Mobile: < 640px
- Tablet: 640-1024px
- Desktop: > 1024px
- Wide: > 1440px

### Mobile-First Approach
1. Design for smallest screen first
2. Add complexity as space allows
3. Touch-friendly targets (44px+)
4. Thumb-zone optimization (bottom 1/3 of screen)

### Common Responsive Patterns
- **Stack to Side** - Vertical on mobile, horizontal on desktop
- **Off-Canvas Menu** - Hamburger menu → full nav
- **Priority+** - Show key items, hide rest in "More"
- **Column Drop** - Multi-column → single column

## Content Strategy

### Readability
- Line length: 50-75 characters
- Line height: 1.4-1.6 for body text
- Paragraph spacing: 1.5x line height
- Left-align body text (easier to scan)

### Writing for UI
- **Labels** - Nouns (Settings, Profile)
- **Buttons** - Verbs (Save, Delete, Continue)
- **Messages** - Clear, concise, helpful
- **Errors** - What went wrong + how to fix

### Microcopy
- Confirmation prompts (Are you sure?)
- Empty states (No items yet. Create one!)
- Success messages (Saved successfully!)
- Tooltips (concise explanations)

## Design Patterns Library

### Modals
- Overlay background (rgba(0,0,0,0.5))
- Center content
- Close button (top-right)
- Escape key to close
- Focus trap (tab stays within modal)

### Dropdowns
- Max height with scroll
- Selected state indicator
- Keyboard navigation (arrows)
- Search for long lists

### Data Tables
- Fixed header row
- Sortable columns
- Pagination or infinite scroll
- Row hover state
- Actions on right side

### Cards
- Consistent padding (16-24px)
- Clear hierarchy (title → content → actions)
- Hover state for clickable cards
- Shadow or border for depth

## Information Architecture

### Navigation Depth
- Keep to 3 levels maximum
- Use breadcrumbs for deep structures
- Provide search for content-heavy sites

### Progressive Disclosure
- Show essential info first
- Expand/accordion for details
- "Learn more" links
- Tooltips for definitions

### Chunking Content
- Group related items (Gestalt principle)
- Use whitespace to separate groups
- Headers to define sections
- No more than 7±2 items per group
