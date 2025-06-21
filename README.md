# Image Background Remover

This is a Streamlit web application that allows users to easily remove backgrounds from their images. It leverages the `rembg` library for efficient background removal and provides a simple, intuitive user interface.

## Features

* **Simple Image Upload:** Upload your image files directly through the web interface.
* **Automatic Background Removal:** Powered by the `rembg` library for accurate background removal.
* **Image Resizing:** Automatically resizes large images to prevent performance issues and optimize processing.
* **Before & After View:** See your original image alongside the background-removed version for easy comparison.
* **Download Processed Image:** Download your new image with a transparent background in PNG format.
* **Progress & Error Handling:** Provides real-time feedback on processing progress and handles potential errors gracefully.

## How to Use

1.  **Run the Application:**
    * Ensure you have Python and `streamlit` and `rembg` installed. You can install them via pip:
        ```bash
        pip install streamlit rembg Pillow
        ```
    * Save the provided Python code as `bg_remove.py`.
    * Run the application from your terminal:
        ```bash
        streamlit run bg_remove.py
        ```
    * This will open the application in your web browser.

2.  **Upload Your Image:**
    * In the sidebar, click on "Upload an image" and select a PNG, JPG, or JPEG file from your computer.

3.  **View and Download:**
    * Once uploaded, the application will process the image, and you will see the original and the fixed image displayed.
    * Click the "Download fixed image" button in the sidebar to save the processed image to your device.

## Image Guidelines and Limitations

* **Supported Formats:** PNG, JPG, JPEG.
* **Maximum File Size:** 10MB. Files larger than this will not be processed.
* **Maximum Image Dimensions:** Images will be automatically resized to a maximum of 2000 pixels on their longest side to ensure efficient processing.
* **Processing Time:** Processing time may vary depending on the size and complexity of the image.

## Dependencies

* `streamlit`
* `rembg`
* `Pillow` (PIL - Python Imaging Library)
* `numpy`
