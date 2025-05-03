# KN Biosciences Landing Page Maintenance Guide

This guide will help you maintain and customize the KN Biosciences Oil Palm Mission landing page. Whether you're new to web development or need a quick reference, follow these detailed instructions.

## Table of Contents
1. [Updating Text and Styling](#updating-text-and-styling)
2. [Managing Links](#managing-links)
3. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains the company name and navigation menu. To update:

```html
<!-- Located at the top of the page -->
<span class="text-xl font-bold text-emerald-500">KN Biosciences</span>
```
- To change the company name, simply replace "KN Biosciences"
- To modify the color, replace `text-emerald-500` with another color (e.g., `text-blue-500`)

### Hero Section
The main headline and subheading are in the first section:

```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold leading-tight mb-8">
    Grow Wealth with Oil Palm: Join KN Biosciences Oilpalm mission Today!
</h1>
<p class="text-xl md:text-2xl text-gray-400 mb-12">
    Transform Your Land, Secure Your Future with Oilpalm Plantation
</p>
```
- Update text between the tags to change content
- Size classes explained:
  - `text-4xl`: Default size
  - `md:text-5xl`: Size on medium screens
  - `lg:text-6xl`: Size on large screens

### Features Section
Each feature card follows this structure:

```html
<div class="bg-gray-800 p-8 rounded-2xl hover:bg-gray-750 transition-all duration-300">
    <div class="text-emerald-500 text-4xl mb-4">💰</div>
    <h3 class="text-xl font-semibold mb-4">Assured Buy-Back Scheme</h3>
    <p class="text-gray-400">Guaranteed purchase of your oil palm produce...</p>
</div>
```
- Replace emoji, heading, and description text as needed
- Keep the class structure intact for consistent styling

## Managing Links

### Navigation Menu Links
Current navigation links are:

```html
<div class="hidden md:flex items-center space-x-8">
    <a href="#features" class="text-gray-300 hover:text-white">Features</a>
    <a href="#benefits" class="text-gray-300 hover:text-white">Benefits</a>
    <a href="#faq" class="text-gray-300 hover:text-white">FAQ</a>
    <a href="wa.link/tiogt2" class="bg-emerald-600 hover:bg-emerald-700">Contact Us</a>
</div>
```

To update links:
1. Internal links (starting with #) connect to page sections
2. Replace `wa.link/tiogt2` with your actual WhatsApp link
3. Format: `href="your-link-here"`

### Contact Links
Located in multiple places:

```html
<!-- WhatsApp Button -->
<a href="wa.link/tiogt2" class="bg-emerald-600 hover:bg-emerald-700">Contact Us on WhatsApp</a>

<!-- Email Link -->
<a href="mailto:oilpalm@knbiosciences.in" class="text-emerald-500 hover:text-emerald-400">oilpalm@knbiosciences.in</a>
```

Update these by replacing:
- WhatsApp link: Change `wa.link/tiogt2` to your actual WhatsApp business link
- Email: Replace `oilpalm@knbiosciences.in` with your email address

## Adding Privacy and Terms Pages

### Step 1: Add Footer Links
Insert these links in the footer section:

```html
<div class="container mx-auto px-4 sm:px-6 lg:px-8">
    <div class="text-center">
        <p class="text-gray-400">© 2024 KN Biosciences. All rights reserved.</p>
        <div class="mt-4">
            <a href="mailto:oilpalm@knbiosciences.in" class="text-emerald-500 hover:text-emerald-400">oilpalm@knbiosciences.in</a>
            <!-- Add these lines below the email -->
            <span class="mx-2 text-gray-400">|</span>
            <a href="privacy.html" class="text-emerald-500 hover:text-emerald-400">Privacy Policy</a>
            <span class="mx-2 text-gray-400">|</span>
            <a href="terms.html" class="text-emerald-500 hover:text-emerald-400">Terms & Conditions</a>
        </div>
    </div>
</div>
```

### Step 2: Create Policy Pages
1. Create two new files: `privacy.html` and `terms.html`
2. Use the same header and footer as `index.html`
3. Add your policy content between the `<main>` tags

## Troubleshooting

Common Issues:
1. **Broken Links**: 
   - Check for typos in `href` attributes
   - Ensure files exist in the correct directory
   - Test all links after updating

2. **Styling Issues**:
   - Keep Tailwind CSS classes together
   - Don't remove responsive classes (starting with `md:` or `lg:`)
   - Maintain the same class order for consistency

3. **Layout Problems**:
   - Verify all opening tags have matching closing tags
   - Keep the container structure intact
   - Don't remove `data-aos` attributes as they control animations

Need help? Contact your web developer or refer to the [Tailwind CSS documentation](https://tailwindcss.com/docs).