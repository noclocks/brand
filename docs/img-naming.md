# Naming Conventions

> Naming conventions for files, folders, and other assets.

## Contents

- [Naming Conventions](#naming-conventions)
  - [Contents](#contents)
  - [Images](#images)
    - [Company or Client Name](#company-or-client-name)
    - [Type or Configuration](#type-or-configuration)
    - [Color Scheme](#color-scheme)
    - [Color Gamut (Space)](#color-gamut-space)

## Images

Images should be named in the following format:

```text
<company>-<type>-<classification>-<fgcolor>-<bgcolor>-<> (<width>x<height>).<extension>
```

### Company or Client Name

- File names should start with the company or client name.
- This can be the full name or an easily recognizable shorthand abbreviation.
- This helps identify the company or client the file is associated with quickly and clarifies whom the file belongs to.

### Type or Configuration

> These are just a few examples of different types of logos. Each type has its own unique characteristics and can be used to create a distinct visual identity for a company or brand.

- Logo Types:
  - **Full (Complete) Logo**: A full logo is a logo that includes the company or brand name along with a symbol or graphic. It is a complete representation of the brand and is often used in various marketing materials.
  - **Wordmark**: A wordmark logo is a logo with the company or brand name written in a unique and stylized font. It focuses on typography to create a memorable and recognizable logo.
  - **Lettermark**: A lettermark logo is a logo that uses the initials or acronyms of the company or brand name to create a unique and recognizable logo.
  - **Brandmark**: A brandmark logo is a logo that uses a symbol or graphic to represent the company or brand without including the company name. It is often used to create a strong visual identity and can be easily recognized even without the company name.
  - **Combination**: A combination logo is a logo that combines different elements such as the company name, symbol, and tagline to create a unique and memorable logo.
  - **Icon**: An icon logo is a logo that uses a simple symbol or graphic to represent a company or brand. It is often used to create a strong visual identity and can be easily recognized even without the company name.
  - **Mascot**: A mascot logo is a logo that uses a character or figure to represent a company or brand. It is often used to create a friendly and approachable brand image.
  - **Emblem**: An emblem logo is a logo that uses a symbol or graphic enclosed within a shape or frame to create a unique and recognizable logo.
  - **Abstract**: An abstract logo is a logo that uses abstract shapes, lines, and colors to create a unique and memorable logo.

### Color Scheme

Indicate the color scheme used in the logo. Whether it's full color, black and white, or transparent, this detail guides users in choosing the right file for their needs.


- File names should include the color scheme used in the design.
- This helps identify the color palette used in the design and clarifies the visual style of the design.
- Whether Full, Black, White, Dark, Light, Transparent, or any other color scheme used in the design.

Examples:

- `full-color`: Full-color logo (original version with all intended colors)

- `grayscale`: This version of the logo uses shades of gray instead of color. It is commonly used for black and white printing or when color is not available.

- `monochrome`: This version of the logo uses a single color, usually black or white, or a specific color from the brand's color palette.

  - `mono-black`: Black logo (optimized for light backgrounds)
  - `mono-white`: White logo (optimized for dark backgrounds)

- `spot-color`: This version of the logo uses specific colors from the brand's color palette. It is commonly used for printing purposes, where only a limited number of colors can be used.

- `reverse`: This version of the logo is designed to be used on a dark background. The colors are inverted to ensure visibility and legibility.

- `transparent`: This version of the logo has a transparent background, allowing it to be placed on any color or image without a visible background.

### Color Gamut (Space)

Mention the **color gamut** used in the file, whether it's `RGB` (for digital use) or `CMYK` (for print). This ensures that users select the correct file for their intended output.

Examples of color gamuts:

- **Monochromatic Gamut:** This gamut consists of various shades and tones of a single color. It often conveys simplicity, elegance, and a clean, modern aesthetic. Examples include logos using various shades of blue or gray.

- **Complementary Gamut:** Complementary colors are opposite each other on the color wheel, such as red and green or blue and orange. Logos using complementary colors can create a sense of balance, contrast, and harmony.

- **Analogous Gamut:** Analogous colors are adjacent to each other on the color wheel, like red, orange, and yellow. Logos using analogous colors can create a feeling of warmth, unity, and a smooth transition between colors.

- **Triadic Gamut:** Triadic colors are evenly spaced around the color wheel, such as red, blue, and yellow. Logos with triadic color schemes are vibrant and can evoke a sense of diversity, energy, and playfulness.

- **Achromatic Gamut:** This gamut uses only black, white, and shades of gray. Achromatic logos often convey simplicity, sophistication, and a timeless quality. They can also be used effectively to emphasize shapes and typography.

- **Custom Gamut:** Some brands create their own unique color gamut by combining specific colors that represent their identity or values. These custom gamuts help brands stand out and convey a distinctive message.

- **Cultural Gamut:** Logos may incorporate colors that have cultural significance. For example, red and gold are often associated with luck and prosperity in Chinese culture, while green is associated with nature and health in many Western cultures.

- **Seasonal Gamut:** Brands may adapt their logo colors according to seasons or holidays. For instance, using pastel colors for spring or red and green for Christmas-themed logos.


### Image Dimensions

The dimensions should be the width and height of the image in pixels.

- The dimensions should be specified by wrapping the `<width>x<height>` in parenthesis and placed at the end of the file name right before the extension (e.g. `(1920x1080).png`).

- If the dimensions are excluded from the file name, this indicates one of two things:

  - The image is a vector image (e.g. SVG) and does not have a fixed width.
  - That file is the "default" size for that image type.

- For example, the `noclocks-logo-main` has two variants based off the colors:

    - `noclocks-logo-main-white-transparent.png`
    - `noclocks-logo-main-black-transparent.png`

- The default dimensions for the `noclocks-logo-main` is `500x500` pixels, but the ` (500x500)` is not included in the file name, because it is the default size.

- In scenarios like this one, ensure that both of the image files are the same size, otherwise include the dimensions in the file name.

### Extension

The extension should be the file extension of the image.

- The extension should be specified using its *name* (e.g. `png`, `jpg`, `svg`, etc.).

- We primarily use the following file extensions:

  - `png`: Portable Network Graphics
  - `jpg` or `jpeg`: Joint Photographic Experts Group
  - `gif`: Graphics Interchange Format
  - `svg`: Scalable Vector Graphics
  - `webp`: Web Picture
  - `avif`: AV1 Image File Format
  - `ico`: Icon
  - `pdf`: Portable Document Format

- On rare occasions, we may also use the following file extensions:
  - `tiff`: Tagged Image File Format
  - `bmp`: Bitmap Image File
  - `eps`: Encapsulated PostScript
  - `psd`: Photoshop Document
  - `ai`: Adobe Illustrator
  - `indd`: Adobe InDesign Document
  - `cdr`: CorelDRAW Image File
  - `sketch`: Sketch File

- The file extension should be chosen based on the intended use of the image and the compatibility with the software or platform where the image will be displayed.

- For example, if the image is intended for use on a website, the `png` or `webp` format may be preferred due to their support for transparency and compression. If the image is intended for print, the `pdf` or `tiff` format may be preferred for high-quality output.

## Example

Applying the naming conventions mentioned above, here is an example of a logo with various types, color schemes, dimensions, and extensions:

- Full Logo with both the logo mark and logotype combined
- Full Color
- High-Resolution Vector Format
- Transparent Background

```text
noclocks-fulllogo-fullcolor-highres-transparent.svg
```

In this example:

- `noclocks`: Company name
- `fulllogo`: Type of logo
- `fullcolor`: Color scheme
- `highres`: High resolution
- `transparent`: Transparent background

The file extension `svg` indicates that it is a vector format suitable for high-resolution output.

By following these naming conventions, users can quickly identify the type, color scheme, dimensions, and format of the image, making it easier to select the right file for their needs.

## Conclusion
