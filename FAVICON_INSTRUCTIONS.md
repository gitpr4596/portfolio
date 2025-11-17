# How to Create Favicon Files for Your Website

Your website is configured to use a favicon (the "PS" logo that appears in browser tabs). You need to create the following image files from your logo:

## Required Favicon Files:

1. **favicon-32x32.png** - 32x32 pixels (standard favicon)
2. **favicon-16x16.png** - 16x16 pixels (small favicon)
3. **apple-touch-icon.png** - 180x180 pixels (for iOS devices)
4. **android-chrome-192x192.png** - 192x192 pixels (for Android)
5. **android-chrome-512x512.png** - 512x512 pixels (for Android)

## Quick Steps:

### Option 1: Online Favicon Generator (Easiest)
1. Go to https://favicon.io/favicon-generator/
2. Upload your logo image (or create one with "PS" text)
3. Download the generated favicon package
4. Extract and copy these files to your portfolio folder:
   - `favicon-32x32.png`
   - `favicon-16x16.png`
   - `apple-touch-icon.png`
   - `android-chrome-192x192.png`
   - `android-chrome-512x512.png`

### Option 2: Create from Your Logo
1. Use an image editor (Photoshop, Canva, GIMP, or online tools)
2. Create a square version of your "PS" logo (dark gray square with white "PS")
3. Resize to each required size:
   - 16x16, 32x32, 180x180, 192x192, 512x512 pixels
4. Save as PNG files with the exact names listed above

### Option 3: Use Your Existing Logo
If you have a high-quality `logo.jpeg` file:
1. Convert it to PNG format
2. Make it square (crop if needed)
3. Resize to the required dimensions
4. Save with the filenames above

## File Format:
- **Format**: PNG (transparent background recommended)
- **Background**: Black or transparent
- **Text**: White "PS" letters
- **Style**: Square with rounded corners (optional)

## After Creating Files:
1. Place all favicon files in the same folder as `index.html`
2. Deploy to Netlify
3. Clear your browser cache
4. Your favicon should appear in browser tabs!

## Testing:
- Open your website in different browsers (Chrome, Firefox, Safari, Edge)
- Check mobile devices (iOS Safari, Android Chrome)
- The favicon should appear in:
  - Browser tabs
  - Bookmarks
  - Browser history
  - Mobile home screen (when saved)

## Notes:
- If files don't appear immediately, clear browser cache (Ctrl+Shift+Delete / Cmd+Shift+Delete)
- Make sure filenames match exactly (case-sensitive)
- PNG format works best for favicons


