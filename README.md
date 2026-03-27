# intake-form

Application for Free Legal Services — an online intake form for SLSLS.

## Replacing the Logo

The logo is displayed at the top of the intake form and is loaded from `assets/logo.svg`.

To replace it with a new image:

1. **Same format (SVG):** Replace the file `assets/logo.svg` with your new SVG file, keeping the same filename.

2. **Different format (PNG, JPG, etc.):** Place your new image file in the `assets/` folder (e.g., `assets/logo.png`), then update the `<img>` tag in `index.html`:

   ```html
   <!-- Change the src and alt attributes as needed -->
   <img src="assets/logo.png" alt="SLSLS Logo" class="logo-img">
   ```

### Logo Guidelines

- **Recommended height:** The logo is displayed at 52px tall; width adjusts automatically.
- **Supported formats:** SVG (recommended), PNG, JPG, WEBP.
- **Transparent background:** Use a transparent background for best results, or ensure the logo background matches the form's white header.