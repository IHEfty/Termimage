# Termimage
This project, written using the [**Tender**](https://github.com/2dprototype/tender-free), converts images to ASCII art and displays them in the terminal with optional color support.

## Requirements

To use this project, you need to install the [**Tender**](https://github.com/2dprototype/tender-free). Clone and install Tender by following the instructions from the Tender GitHub repository:

```
git clone https://github.com/2dprototype/tender-free.git
cd tender-free
```

## Running the Project

Once you have Tender installed, you can run the project using `cli.td`. Here's how:

```
tender cli.td
```

This will render the embedded image `download.jpg` as ASCII art in the terminal.

### Customizing the Image

To display a different image, replace `download.jpg` with the name of your own image file. Make sure the image is saved in the same folder as the script.

Example:

```tender
data := embed("your_image.jpg")
sysout t.to_ascii(data, 40, 30, true)
```

Feel free to modify the width, height, and whether color is enabled by adjusting the parameters in the script.

## Files

- **termcolor.td**: Provides utilities for matching RGB values to ANSI color codes.
- **termimage.td**: Contains the logic for decoding an image and converting it to ASCII art.
- **cli.td**: The main script that processes and displays an embedded image.

Enjoy experimenting with different images and settings!

---
