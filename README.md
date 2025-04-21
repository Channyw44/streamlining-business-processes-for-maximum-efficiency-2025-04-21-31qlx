# Landing Page Maintenance Guide
## Willaby Solutions Website Documentation

This guide provides detailed instructions for maintaining and customizing the Willaby Solutions landing page. It's designed for beginners with no prior coding experience.

## Table of Contents
1. [Updating Text and Styling](#updating-text-and-styling)
2. [Managing Links](#managing-links)
3. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Main Sections to Update

#### Header/Navigation
```html
<a href="/" class="text-2xl font-bold bg-gradient-to-r from-purple-500 to-pink-500 bg-clip-text text-transparent">
    Willaby Solutions
</a>
```
To change the company name:
1. Locate this code in the header section
2. Replace "Willaby Solutions" with your desired text
3. Keep the surrounding HTML tags and classes intact

#### Hero Section
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold leading-tight mb-8 bg-gradient-to-r from-purple-400 to-pink-400 bg-clip-text text-transparent">
    Streamlining Business Processes for Maximum Efficiency
</h1>
```
To modify the main headline:
1. Find this `<h1>` tag in the hero section
2. Change the text while preserving the HTML tags
3. The classes control:
   - `text-4xl`: Base text size
   - `md:text-5xl`: Tablet text size
   - `lg:text-6xl`: Desktop text size
   - `bg-gradient-to-r`: Creates the gradient effect

### Tailwind CSS Class Guide

Key classes used throughout:
- Text sizes: `text-sm`, `text-base`, `text-lg`, `text-xl`, `text-2xl`, etc.
- Colors: 
  - Background: `bg-gray-900`, `bg-purple-500`
  - Text: `text-gray-100`, `text-gray-400`
- Spacing:
  - Margin: `m-4`, `mb-8`, `my-4`
  - Padding: `p-4`, `px-6`, `py-24`

Example of updating a feature card:
```html
<div class="bg-gray-800 rounded-xl p-8 hover:scale-105 transform transition duration-300 shadow-lg hover:shadow-purple-500/25">
    <h3 class="text-xl font-semibold mb-4">24/7 Availability</h3>
    <p class="text-gray-400">Always-on support and service availability when you need it most</p>
</div>
```

## Managing Links

### Navigation Menu Links
Current navigation links:
```html
<div class="hidden md:flex space-x-8">
    <a href="#features" class="hover:text-purple-400 transition-colors duration-300">Features</a>
    <a href="#benefits" class="hover:text-purple-400 transition-colors duration-300">Benefits</a>
    <a href="#faq" class="hover:text-purple-400 transition-colors duration-300">FAQ</a>
    <a href="#contact" class="hover:text-purple-400 transition-colors duration-300">Contact</a>
</div>
```

To update links:
1. Locate the `href` attribute
2. For internal sections, use `#section-name`
3. For external links, use full URL: `https://example.com`

### Call-to-Action Button
```html
<a href="https://www.willabysolutions.com" class="inline-block bg-gradient-to-r from-purple-500 to-pink-500 text-white font-semibold px-8 py-4 rounded-lg hover:scale-105 transform transition duration-300 shadow-lg hover:shadow-purple-500/25">
    Get Started Today
</a>
```
To update:
1. Change the `href` value to your desired URL
2. Modify button text between the opening and closing tags

## Adding Privacy and Terms Pages

### Current Footer Links
```html
<div>
    <h4 class="font-semibold mb-4">Legal</h4>
    <ul class="space-y-2 text-gray-400">
        <li><a href="#" class="hover:text-purple-400 transition-colors duration-300">Privacy Policy</a></li>
        <li><a href="#" class="hover:text-purple-400 transition-colors duration-300">Terms of Service</a></li>
    </ul>
</div>
```

To link privacy and terms pages:
1. Create `privacy.html` and `terms.html` in your website directory
2. Update the href attributes:
```html
<li><a href="privacy.html" class="hover:text-purple-400 transition-colors duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="hover:text-purple-400 transition-colors duration-300">Terms of Service</a></li>
```

## Troubleshooting

Common issues and solutions:

1. **Broken Links**
   - Check for typos in `href` attributes
   - Ensure file names match exactly
   - Verify file locations in your directory

2. **Styling Issues**
   - Don't remove classes unless you're sure of their purpose
   - Keep responsive classes (`md:`, `lg:`) to maintain mobile compatibility
   - Maintain the gradient classes for consistent branding

3. **Layout Problems**
   - Preserve the container classes: `container mx-auto`
   - Keep the grid structure: `grid grid-cols-1 md:grid-cols-3`
   - Don't remove padding/margin classes without replacement

Need help? Contact technical support or refer to the [Tailwind CSS documentation](https://tailwindcss.com/docs).