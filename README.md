# QR Code Generator

This Python script generates a QR code based on user input and saves it as an image file. It uses the `qrcode` library for QR code generation.

## Features

- Customizable QR code size and border padding.
- Allows user to input text dynamically for the QR code content.
- Saves the QR code as a PNG image with customizable foreground and background colors.

## Requirements

- Python 3.6 or later
- `qrcode` library
- `Pillow` library (automatically installed with `qrcode`)

## Installation

1. Clone the repository or download the script.

2. Install the required libraries:
   ```bash
   pip install qrcode[pil]
Ensure you have Python installed. You can check your Python version using:
bash
Copy code
python --version
Usage
Run the script:

bash
Copy code
python main.py
Enter the text you want to encode in the QR code when prompted.

The script generates a QR code and saves it as sample.png in the current directory.

You can customize the following:

Size: Change the size parameter in the MyQR class constructor to modify the box size of the QR code.
Padding: Adjust the padding parameter for the border width.
File Name: Modify the file_name parameter in the create_qr method to change the output file name.
Colors: Use the fg and bg parameters in the create_qr method to customize foreground and background colors.
Code Explanation
MyQR Class
Initializes the QR code generator with a customizable size and padding.
Contains the create_qr method to generate and save the QR code.
main() Function
Creates an instance of the MyQR class with default size and padding.
Prompts the user for input, generates a QR code, and saves it as sample.png.
Example Output
If you enter Hello, World! as input, the script will generate a QR code that encodes this text and save it as sample.png.

Notes
The generated QR code image can be scanned using any QR code scanner.
Ensure the file name for the QR code ends with .png for proper image generation.
Contributing
Feel free to fork this repository, make enhancements, and create pull requests!

License
This project is licensed under the MIT License. See the LICENSE file for more details.