# The Concurrent Contractor™ - Branding Guide

## Overview

This document outlines the brand identity for The Concurrent Contractor™ application, including logo usage, color palette, and typography guidelines.

## Logo Files

The application uses three primary logo variations:

### 1. TCC Icon Logo (`tcc-logo.png`)
- **Location**: `assets/images/tcc-logo.png`
- **Usage**: Header navigation, favicon, app icons
- **Description**: Gold gradient TCC letter-mark logo
- **Recommended Size**: 200x200px minimum
- **Format**: PNG with transparent background

### 2. Text Logo - Black (`tcc-text-logo-black.png`)
- **Location**: `assets/images/tcc-text-logo-black.png`
- **Usage**: Documents, alternative headers, light backgrounds
- **Description**: "The Concurrent Contractor™" in serif typeface, black text
- **Format**: PNG with transparent background

### 3. Text Logo - Framed (`tcc-text-logo-framed.png`)
- **Location**: `assets/images/tcc-text-logo-framed.png`
- **Usage**: Reports, presentations, formal documents
- **Description**: "The Concurrent Contractor™" with gold border frame
- **Recommended Size**: 400-600px wide
- **Format**: PNG with white or transparent background

## Color Palette

### Primary Colors

- **Gold (Bright)**: `#FFD700`
  - Usage: Highlights, accents, active states

- **Gold (Dark)**: `#D4AF37`
  - Usage: Gradient starts, subtle accents

- **Gold Gradient**: `linear-gradient(135deg, #D4AF37 0%, #FFD700 100%)`
  - Usage: Logo effects, premium UI elements, text highlights

### Secondary Colors

- **Orange**: `#FF8C00`
  - Usage: CTA buttons, important highlights, active tabs
  - Hover states and emphasis elements

### Neutral Colors

- **Pure Black**: `#000000`
  - Usage: Primary background, high contrast text

- **Dark Gray**: `#1A1A1A`
  - Usage: Card backgrounds, secondary surfaces

- **Medium Gray**: `#333333`
  - Usage: Borders, dividers

- **Light Gray**: `#666666`
  - Usage: Secondary text, disabled states

- **White**: `#FFFFFF`
  - Usage: Primary text on dark backgrounds, report backgrounds

## Typography

### Primary Font Family
```css
font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Helvetica Neue', Arial, sans-serif;
```
- Usage: Body text, UI elements, forms

### Display Font (Headings & Branding)
```css
font-family: Georgia, 'Times New Roman', serif;
```
- Usage: "The Concurrent Contractor™" branding text
- Gives professional, established appearance matching the logo

## Logo Usage Guidelines

### Header Implementation
- TCC icon logo on the left (60px height on desktop, 50px on mobile)
- Text "The Concurrent Contractor™" in serif font with gold gradient
- Black background with gold bottom border

### Report Implementation
- Framed text logo centered at top (max 400px wide)
- Clear space around logo (minimum 1.5rem margin)
- Always on white background for reports

### Favicon
- Uses TCC icon logo (`tcc-logo.png`)
- Automatically scaled by browser

## Responsive Behavior

### Desktop (> 768px)
- Header: Horizontal layout with logo left-aligned
- Logo: 60px height
- Text: Full size (2rem)

### Mobile (≤ 768px)
- Header: Vertical stack, centered
- Logo: 50px height
- Text: Reduced size (1.5rem)
- Report logo: Max 280px width

## Brand Voice

The branding conveys:
- **Professionalism**: Serif typography, refined color palette
- **Premium Quality**: Gold gradient effects, high contrast
- **Trust & Stability**: Classic design elements, consistent structure
- **Modern Efficiency**: Clean UI, streamlined experience

## File Structure

```
concurrent-contractor-app/
├── assets/
│   └── images/
│       ├── tcc-logo.png              # Icon logo
│       ├── tcc-text-logo-black.png   # Text logo (black)
│       ├── tcc-text-logo-framed.png  # Text logo (framed)
│       └── README.md                  # Image specifications
├── index.html                         # Main application
└── BRANDING.md                        # This file
```

## Implementation Notes

1. **Logo fallbacks**: All logo `<img>` tags include `onerror` handlers to gracefully degrade if image files are missing

2. **Gradient text**: The gold gradient on "CONTRACTOR" uses CSS background-clip for modern browsers:
   ```css
   background: var(--gold-gradient);
   -webkit-background-clip: text;
   -webkit-text-fill-color: transparent;
   background-clip: text;
   ```

3. **Accessibility**: Maintain sufficient contrast ratios:
   - White text on black background: 21:1 (AAA)
   - Gold on black: 10:1 (AA for large text)

## Next Steps

To complete the branding implementation:

1. Save the three logo PNG files to `assets/images/` directory:
   - `tcc-logo.png`
   - `tcc-text-logo-black.png`
   - `tcc-text-logo-framed.png`

2. Verify logo display in:
   - Header navigation
   - Report preview
   - Browser favicon

3. Test responsive behavior on mobile devices

4. Generate high-resolution versions for print materials if needed

---

**The Concurrent Contractor™** - OPERATE Framework © 2025
