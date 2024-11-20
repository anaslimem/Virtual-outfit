Virtual Try-On with AI Models
This repository allows users to upload images of garments (top and bottom) and a model image, and visually try on the garments using AI-based virtual try-on models. The application supports a selection of pre-trained AI models and garments, providing an interactive interface where users can view the results instantly.

Features
AI Models for Virtual Try-On: The repository includes various AI models (e.g., Eva, Rouyan, Simon, Xuanxuan, Yaqi, Yifeng) that can simulate the effect of wearing different garments.
Image Upload: Users can upload their garment images (top and bottom) and a base model image for the try-on simulation.
Try-On Simulation: The application processes the garment and model images and displays the resulting image where the garments are virtually "worn" by the model.
Pre-trained Model Support: Easily switch between multiple AI models for different try-on styles.
Installation
To run this project, ensure the following dependencies are installed:

bash
Copy code
pip install opencv-python numpy Pillow requests gradio
You will also need the pre-trained models and garment images for the demo. The models are stored in the models/ directory, and garment images are in the garments/ folder.

Code Overview
Model Selection: The MODEL_MAP dictionary maps different model names to their respective images. The selected model is used to perform the virtual try-on.
Watermark: A watermark is added to the output images to indicate the app is powered by OutfitAnyone.
Image Encoding & API Integration: The garment images are encoded into base64 format and sent to a server (configured via OA_IP_ADDRESS environment variable) for processing.
Gradio Interface: The user interface is built using Gradio, allowing users to interactively upload images, select models, and visualize results.
Examples: Example images are provided for users to test different garment combinations with various AI models.
How to Use
Upload Images: Select a base model image and top and bottom garment images.
Choose a Model: Select the AI model you wish to use for the virtual try-on simulation.
Run the Simulation: Click the "Run" button to see the result of the garment try-on.
View Results: The result will be displayed in the output gallery with the watermark.
Example Workflow
The demo includes a few examples to get started:

Base Model Image: A model image to try on the garments.
Garment Images: Various garment images (e.g., top and bottom pieces).
Result: A result image showcasing the virtual try-on.
File Structure
demo.py: Main Python script containing the logic for the virtual try-on, model selection, and Gradio interface.
models/: Directory containing the pre-trained AI model images.
garments/: Folder containing sample garment images for try-on.
examples/: Folder containing example images for testing

