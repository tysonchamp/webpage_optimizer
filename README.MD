# Image Optimizer

A simple Python script to optimize images by converting them to WebP format, Autometically update them into HTML & CSS and also minifying CSS files.

## Usage

Run the script in your terminal/command prompt. The script will ask you to select the directory containing the images to be optimized. Once the directory is selected, the script will create a new directory with the suffix `_output` containing the optimized images.

## Features

The script optimizes images by:

1. **Converting images to WebP format**: The script converts all `.png`, `.jpg`, and `.jpeg` files in the input directory to `.webp` files, which are smaller in size and provide better compression.
2. **Minifying HTML, CSS files**: The script minifies all `.html` and `.css` files in the input directory to reduce their size.
3. **Updating image references in HTML files**: The script updates the `src` attribute of all `<img>` tags in the HTML files to use `.webp` images if available.
4. **Adding `alt` attribute to all images**: The script adds `alt` attribute to all images in the HTML files with the webpage title.

## How it works

The script uses the following libraries:

1. `tkinter` for creating a graphical user interface (GUI)
2. `pyautogui` for selecting the input directory
3. `Pillow` for converting images to WebP format
4. `csscompressor` for minifying CSS files
5. `BeautifulSoup` for parsing HTML files

## Supported image formats

The script supports the following image formats:

1. `.png`
2. `.jpg`
3. `.jpeg`

## Known issues

1. The script may not work on MacOS if the default web browser is not Google Chrome.
2. The script assumes that the input directory has the same structure as the output directory. If the input directory has sub-directories, the script will not create the sub-directories in the output directory.

## Contributing

If you encounter any issues or have suggestions for new features, feel free to create a pull request or open an issue.

