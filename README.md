
# ImageToA4PDF

## Overview
**ImageToA4PDF** is a simple Python tool that allows you to batch combine images from a folder into A4-sized PDFs. It can also resize existing PDFs to A4 dimensions, ensuring they are standardized. The tool saves the resulting PDFs in both the original folder and an optional separate folder.

## Features
- **Batch Image to PDF Conversion**: Combines multiple images from a folder into a single A4-sized PDF.
- **PDF Resizing**: Resizes existing PDFs to A4 dimensions without cropping the content.
- **Multiple Saving Locations**: Option to save resized PDFs in both the original folder and a separate folder.
- **Skips Corrupted Files**: Automatically skips files that are incomplete or corrupted during processing.

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/ImageToA4PDF.git
   cd ImageToA4PDF
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Ensure that you have the necessary libraries, like:
   - `PyPDF2`
   - `natsort`
   - `reportlab`

You can install them manually if needed:
```bash
pip install PyPDF2 natsort reportlab
```

## Usage

1. **Converting Images to A4-Sized PDF**:
   Place your images in a folder, then run the script to combine them into an A4-sized PDF:

   ```bash
   python convert_images_to_pdf.py --input_folder /path/to/your/images --output_folder /path/to/output
   ```

2. **Resizing Existing PDFs to A4**:
   Run the script to resize PDFs from an input folder to A4 size:

   ```bash
   python resize_pdfs_to_a4.py --input_folder /path/to/your/pdfs --output_folder /path/to/output
   ```

   If you want to save the resized PDFs in the same folder:
   ```bash
   python resize_pdfs_to_a4.py --input_folder /path/to/your/pdfs --output_folder /path/to/your/pdfs
   ```

### Arguments:
- `--input_folder`: Path to the folder containing images or PDFs to process.
- `--output_folder`: Path to the folder where the resized or combined PDFs will be saved.

## Example
To combine images from a folder named `images` and save the resulting PDF to an `output` folder:
```bash
python convert_images_to_pdf.py --input_folder ./images --output_folder ./output
```

To resize PDFs to A4 size and save them to the same folder:
```bash
python resize_pdfs_to_a4.py --input_folder ./pdfs --output_folder ./pdfs
```

## License
This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International License**. See the [LICENSE](LICENSE) file for more details.

## Contributing
If you'd like to contribute to this project, feel free to open a pull request. For major changes, please open an issue first to discuss what you would like to change.

## Issues
If you encounter any issues or bugs, feel free to open an issue in the repository or contact me directly.

## Acknowledgements
Special thanks to the following libraries:
- **PyPDF2** for PDF processing
- **natsort** for natural sorting of files
- **reportlab** for PDF generation
