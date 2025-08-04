# Gonzales Towing Landing Page - Maintenance Guide

This guide will help you maintain and customize the Gonzales Towing landing page. It's written for beginners with no prior coding experience.

## Table of Contents
- [Updating Text and Styling](#updating-text-and-styling)
- [Managing Links](#managing-links)
- [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
- [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains the company name and navigation menu. To update:

1. Company Name:
```html
<div class="text-2xl font-bold text-gray-800">Gonzales Towing</div>
```
Simply replace "Gonzales Towing" with your desired text.

### Hero Section
Located at the top of the page with the main headline:

```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 mb-6">Best Gonzales Towing Service</h1>
<p class="text-xl md:text-2xl text-gray-600 mb-8">Best & Most Reliable Towing Service In Gonzales and Beyond</p>
```

The text sizes are responsive:
- `text-4xl`: Default size
- `md:text-5xl`: Medium screens
- `lg:text-6xl`: Large screens

### Services Section
Each service card follows this structure:
```html
<div class="bg-white rounded-xl shadow-lg p-8 hover:shadow-xl transition duration-300">
    <div class="text-blue-600 mb-4">
        <i class="fas fa-truck-pickup text-4xl"></i>
    </div>
    <h3 class="text-xl font-bold text-gray-900 mb-4">Emergency Service</h3>
    <p class="text-gray-600">24/7 emergency towing service when you need it most.</p>
</div>
```

To modify:
1. Change the icon: Update `fa-truck-pickup` with any [Font Awesome icon](https://fontawesome.com/icons)
2. Update the heading: Replace "Emergency Service" text
3. Update the description: Modify the paragraph text

## Managing Links

### Navigation Menu Links
Current navigation links are:
```html
<div class="hidden md:flex space-x-8">
    <a href="#services" class="text-gray-600 hover:text-blue-600 transition duration-300">Services</a>
    <a href="#benefits" class="text-gray-600 hover:text-blue-600 transition duration-300">Benefits</a>
    <a href="#faq" class="text-gray-600 hover:text-blue-600 transition duration-300">FAQ</a>
    <a href="#contact" class="text-gray-600 hover:text-blue-600 transition duration-300">Contact</a>
</div>
```

To update a link:
1. Locate the `<a>` tag
2. Change the `href` attribute
3. Update the link text

Example:
```html
<a href="#new-section" class="text-gray-600 hover:text-blue-600 transition duration-300">New Section</a>
```

### Social Media Links
The Facebook link appears in multiple places:
```html
<a href="https://www.facebook.com/CharlesDupuis126" class="inline-block bg-blue-600 text-white px-8 py-4 rounded-lg">
```

To update:
1. Replace the Facebook URL with your social media profile
2. Update any reference text

## Adding Privacy and Terms Pages

### Step 1: Create New Files
Create two new files in your website folder:
- `privacy.html`
- `terms.html`

### Step 2: Update Footer Links
Locate these lines in the footer:
```html
<div>
    <h3 class="text-xl font-bold mb-4">Legal</h3>
    <div class="space-y-2">
        <p class="text-gray-400">Privacy Policy</p>
        <p class="text-gray-400">Terms of Service</p>
    </div>
</div>
```

Replace with:
```html
<div>
    <h3 class="text-xl font-bold mb-4">Legal</h3>
    <div class="space-y-2">
        <a href="privacy.html" class="text-gray-400 hover:text-white transition duration-300">Privacy Policy</a>
        <a href="terms.html" class="text-gray-400 hover:text-white transition duration-300">Terms of Service</a>
    </div>
</div>
```

## Troubleshooting

### Common Issues

1. **Broken Links**
   - Check that all `href` attributes point to valid pages
   - Ensure section IDs match their corresponding links
   - Verify file names and paths are correct

2. **Responsive Design Issues**
   - Don't remove `md:` or `lg:` prefixes from classes
   - Keep the viewport meta tag in the header
   - Test on different screen sizes

3. **Icon Problems**
   - Verify Font Awesome is properly loaded
   - Check icon names against Font Awesome documentation
   - Ensure proper icon class prefix (`fas`, `fab`, etc.)

### Need Help?
- Double-check your changes against the original code
- Use browser developer tools (F12) to inspect elements
- Validate your HTML at [W3C Validator](https://validator.w3.org/)

Remember to always make a backup of your files before making changes!