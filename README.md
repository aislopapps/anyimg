Git Hosted: https://sub0kanzai.github.io/AnyIMG_Converter/


AnyIMG Converter


Convert images between formats quickly, right in your browser.
I wanted a way to convert images fast and add free... so I got AI to 100% vibe code this for me.

AnyIMG Converter is a lightweight, single-page image conversion tool. Add one image or a batch, choose an output format, adjust the conversion settings, and download the converted files individually or together as a ZIP archive.
Features
- Browser-based processing: images are decoded and converted in your browser; the app does not upload image files to an AnyIMG server.
- Add images your way: browse for files, drag and drop them, or paste image files from your clipboard.
- Batch conversion: queue multiple images and convert them together.
- Output formats: JPEG, PNG, WebP, AVIF, BMP and ICO. Availability is detected at runtime; AVIF is enabled when its encoder loads successfully.
- Quality control: adjust quality for lossy formats.
- Resize option: set a maximum image dimension while preserving the aspect ratio. Leave it blank to keep the original dimensions.
- Background colour: choose the colour used when transparency must be flattened for JPEG or BMP.
- Download options: save each converted image separately or download all completed conversions as a ZIP file.
- Responsive dark interface: designed for desktop and mobile screens.

No account required: the current standalone app has no sign-in flow.
Supported formats and limitations
Output formats
Format	Notes
JPEG	Lossy; transparency is flattened using the selected background colour.
PNG	Lossless; supports transparency.
WebP	Supports transparency; quality setting is available.
AVIF	Uses a WebAssembly encoder loaded on demand from esm.sh. AVIF is unavailable if the encoder cannot load.
BMP	Uses the app's built-in encoder; transparency is flattened using the selected background colour.
ICO	Created from a PNG image and resized to a maximum side of 256 pixels.


Input files
The file picker accepts common image files, including JPG/JPEG, PNG, GIF, WebP, SVG, AVIF, BMP, ICO and TIFF. Actual decoding depends on the browser's image support. A file appearing in the queue does not guarantee that the browser can decode it.

Known limitations
- Animated GIF and animated WebP files are converted from their first frame only. This tool does not preserve animation.
- Transparency is flattened for JPEG and BMP. Choose the background colour before converting those formats.
- AVIF conversion requires the AVIF encoder module to load from esm.sh; a network connection is needed for that dependency. Other supported formats can still work if AVIF is unavailable.
- Output format availability can vary with browser support.
- Large images and large batches require memory and processing power in the device's browser. Performance depends on the device and browser.
- This is a client-side converter, not an image editor or a cloud storage service.
Use it
Run locally
1. Download or clone this repository.
2. Open index.html in a modern browser.
3. Drop images into the upload area, click it to browse, or paste image files from the clipboard.
4. Choose the output format and adjust quality, maximum dimension and background colour as needed.
5. Click Convert all.
6. Download an individual result or click Download ZIP to save all completed conversions together.
No build step, package manager or application server is required for the current standalone version.
Publish it as a static website
AnyIMG is a static HTML/CSS/JavaScript app and can be hosted by a static website provider.


Contributing
Suggestions, bug reports and improvements are welcome. When reporting a conversion issue, include:
- Your browser and operating system.
- The input file format and approximate file size.
- The output format you selected.
- Any error message shown by the app.
Please do not upload private or sensitive images in public issue reports.


MIT License

Copyright (c) 2026 Sub0Kanzai

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
