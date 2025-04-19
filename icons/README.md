# Money Bag and Coins Stack Web Icon

This directory contains icon assets for the web app, updated to use a design that matches the provided money bag and coins stack image for the Jubba (جُعبه) financial app.

## Implementation Details

The primary web app icon has been precisely recreated as an SVG version of the provided image featuring:
- A stack of blue coins with light blue/white centers
- A money bag with a light blue fill and blue outline
- A dollar sign in the center of the money bag
- Blue tie and strings at the top of the money bag

This design accurately recreates the provided icon as a scalable vector graphic that looks crisp on all devices while clearly conveying the app's financial purpose.

### Files Added/Modified:

1. `/web/favicon.svg` - Vector-based money bag and coins SVG that serves as the primary favicon
2. `/web/index.html` - Updated to include inline SVG favicon and dynamic favicon generation code
3. `/web/manifest.json` - Updated to reference the SVG icon and appropriate theme colors

### Advantages of SVG Favicon

- **Exact Recreation**: The SVG faithfully reproduces the provided icon design
- **Scalability**: SVG icons scale to any size without losing quality
- **Dynamic Generation**: Favicon is generated at runtime from SVG code
- **Modern Browsers**: All modern browsers support SVG favicons

### Fallbacks

For browsers that don't support SVG favicons, a PNG fallback has been provided.

## How to Generate PNG Icons From SVG (Manual Steps)

If you need to generate PNG versions of the SVG icon for various sizes (192px, 512px, etc.), you can use any of these methods:

1. **Using Inkscape (Free):**
   ```
   inkscape favicon.svg --export-png=icons/money-bag-192.png -w 192 -h 192
   inkscape favicon.svg --export-png=icons/money-bag-512.png -w 512 -h 512
   ```

2. **Using ImageMagick (Free):**
   ```
   convert -background none -size 192x192 favicon.svg icons/money-bag-192.png
   convert -background none -size 512x512 favicon.svg icons/money-bag-512.png
   ```

3. **Using Online Converters:**
   - Upload the SVG to services like [Convertio](https://convertio.co/svg-png/) or [SVG2PNG](https://svgtopng.com/)
   - Select the desired dimensions for output

After generating the PNGs, update the manifest.json to point to these new files.

## Theme Colors

The theme color has been set to match the blue color (#4285F4) from the provided icon design. 