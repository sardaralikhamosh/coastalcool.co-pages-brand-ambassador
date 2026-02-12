# Brand Ambassador Page - Shopify Sections Implementation Guide

## Overview
This package contains 6 Shopify sections to create a complete Brand Ambassador page with your custom pink theme color: `hsl(333.39deg 80.42% 71.96%)`

## Sections Included

### 1. **section-1-hero-join-crew.liquid**
- Hero section with logo, title, description, CTA button
- Includes "Already a member? Log in" link
- Customizable through Shopify theme editor

### 2. **section-2-circular-gallery.liquid**
- 4 circular images in a responsive grid
- Hover effects with pink accent color
- Perfect for showcasing brand ambassadors

### 3. **section-3-partnership-opportunities.liquid**
- Title and customizable tags
- Interactive image carousel with navigation
- Video play button support
- Fully responsive carousel

### 4. **section-4-one-pound-promise.liquid**
- Statistics section with pink background
- 3 stats with icons (bottle, package, sun)
- Animated fade-in effects
- Environmental impact showcase

### 5. **section-5-features.liquid**
- 5 feature boxes with icons
- Icons: shipping, lock, headphones, palm tree, award
- Hover effects and responsive grid

### 6. **section-6-instagram-gallery.liquid**
- Instagram-style image grid
- "Follow Us" button with Instagram icon
- Hover overlay effects with pink gradient
- 6 images in responsive grid

## Installation Instructions

### Step 1: Upload Custom CSS File (IMPORTANT!)

1. **Upload brand-ambassador-styles.css**
   - Go to: Online Store → Themes → Edit code
   - In the left sidebar, find the "Assets" folder
   - Click "Add a new asset"
   - Upload `brand-ambassador-styles.css`
   - Save

2. **Link CSS in theme.liquid**
   - In "Layout" folder, open `theme.liquid`
   - Add this line in the `<head>` section:
   ```liquid
   <link rel="stylesheet" href="{{ 'brand-ambassador-styles.css' | asset_url }}">
   ```
   - Save the file

### Step 3: Upload Section Files to Shopify

1. **Access your Shopify Admin**
   - Log in to your Shopify store admin panel

2. **Navigate to Theme Files**
   - Go to: Online Store → Themes
   - Click "Actions" → "Edit code" on your active theme

3. **Upload Each Section**
   - In the left sidebar, find the "Sections" folder
   - Click "Add a new section"
   - Copy the content from each `.liquid` file
   - Name them exactly as shown:
     - `section-1-hero-join-crew`
     - `section-2-circular-gallery`
     - `section-3-partnership-opportunities`
     - `section-4-one-pound-promise`
     - `section-5-features`
     - `section-6-instagram-gallery`
   - Save each section

### Step 4: Create the Brand Ambassador Page Template

1. **Create a New Page Template**
   - In the Theme Editor, go to "Templates"
   - Click "Add a new template"
   - Select "page" as the template type
   - Name it: `page.brand-ambassador`

2. **Add Sections to Template**
   - In the page template editor, click "Add section"
   - Add the sections in this order:
     1. Brand Ambassador Hero
     2. Circular Images Gallery
     3. Partnership Opportunities
     4. One Pound Promise
     5. Features Section
     6. Instagram Gallery

3. **Create the Page**
   - Go to: Online Store → Pages
   - Click "Add page"
   - Title: "Brand Ambassador" (or your preferred title)
   - In the right sidebar, under "Template", select "page.brand-ambassador"
   - Save the page

### Step 5: Customize Content

#### Section 1: Hero
- Upload your logo image
- Edit title: "JOIN THE CREW"
- Update description text
- Set CTA button link (application form URL)
- Configure login link

#### Section 2: Circular Gallery
- Add 4 images of brand ambassadors
- Images should be square (at least 400x400px)
- Add descriptive alt text

#### Section 3: Partnership Opportunities
- Add tags: "Discount codes", "Additional opportunities", "Gifting", etc.
- Upload 5+ carousel images (portrait orientation recommended)
- Mark videos with play button checkbox
- Images should be at least 600x840px

#### Section 4: One Pound Promise
- Customize the 3 statistics:
  - Number (e.g., "75,000+")
  - Label (e.g., "Plastic Bottles Removed")
  - Select appropriate icon
- Background color is automatically pink

#### Section 5: Features
- Add 5 features with:
  - Icon selection
  - Title
  - Description
- Covers: shipping, checkout, support, vacation vibe, quality

#### Section 6: Instagram Gallery
- Upload 6+ Instagram-style images (square format)
- Images should be at least 500x500px
- Set your Instagram profile URL
- Customize "Follow Us" button text

## Design Features

### Color Scheme - ALOESUN Brand Colors
- **Primary Brand Color**: `hsl(333.39deg 80.42% 71.96%)` (Pink #f181b2)
- **Hover State**: `hsl(333.39deg 80.42% 65%)` (Slightly darker pink)
- **Text Primary**: `#2e2a39` (Dark gray, matching ALOESUN)
- **Text Secondary**: `#666666` (Medium gray)
- **Gradients**: Pink gradient overlays on hover effects

### Typography - Poppins Font Family
All sections use the **Poppins** font family to match your ALOESUN website:
- **Headers**: Poppins Bold (700 weight)
- **Body Text**: Poppins Regular (400 weight)
- **Buttons/Links**: Poppins Semibold (600 weight)
- **Tags**: Poppins Medium (500 weight)

**Font Sizes:**
- Main Titles: 32-48px
- Section Titles: 28-36px  
- Subheadings: 14-16px
- Body Text: 15px
- Small Text: 13-14px

### Design Elements
- **Button Style**: 10px border radius (matching ALOESUN)
- **Rounded corners**: 10-12px on cards and elements
- **Shadows**: Soft pink-tinted shadows on hover
- **Transitions**: Smooth 0.3s ease on all interactive elements

### Responsive Design
All sections are fully responsive with breakpoints at:
- Desktop: 1200px+
- Tablet: 768px - 1199px
- Mobile: < 768px

### Animations & Effects
- Hover lift effects on cards
- Smooth color transitions
- Fade-in animations on statistics
- Carousel smooth sliding
- Instagram overlay effects

## Customization Tips

### Changing Colors
To adjust the pink color throughout all sections:
1. Search for `hsl(333.39deg 80.42% 71.96%)`
2. Replace with your desired color
3. Maintain consistency across all sections

### Image Recommendations
- **Hero Logo**: 100x100px, transparent PNG
- **Circular Gallery**: 400x400px, square
- **Partnership Carousel**: 600x840px, portrait
- **Instagram Grid**: 500x500px, square

### Font Customization
To use custom fonts:
1. Upload fonts to Assets folder in theme
2. Update font-family in CSS
3. Ensure fallback fonts are included

## Browser Support
- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome)

## Accessibility Features
- Alt text support for all images
- Keyboard navigation for carousel
- Semantic HTML structure
- ARIA labels where appropriate
- Color contrast ratios meet WCAG standards

## Performance Optimization
- Lazy loading images
- Optimized SVG icons
- CSS-only animations
- Minimal JavaScript
- Responsive images

## Troubleshooting

### Sections not appearing?
- Ensure section files are named correctly
- Check that sections are added to the page template
- Clear browser cache

### Images not displaying?
- Verify image uploads in section settings
- Check image file formats (JPG, PNG, WebP)
- Ensure image URLs are valid

### Carousel not working?
- Check JavaScript is enabled
- Verify section has at least 4 images
- Try refreshing the page

### Colors not matching?
- Double-check HSL color value
- Clear Shopify theme cache
- Force refresh browser (Ctrl+Shift+R)

## Support

For additional customization or support:
1. Check Shopify theme documentation
2. Test in Shopify preview mode first
3. Use browser developer tools to debug CSS
4. Verify all section settings are configured

## Version Information
- **Created**: January 2026
- **Shopify Compatibility**: 2.0+
- **Theme Requirements**: Online Store 2.0 compatible

---

**Note**: Always backup your theme before making changes. Test thoroughly in a preview environment before publishing to live site.
