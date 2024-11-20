# Virtual Try-On with AI Models

This repository allows users to upload images of garments (top and bottom) and a model image, and visually try on the garments using AI-based virtual try-on models. The application supports a selection of pre-trained AI models and garments, providing an interactive interface where users can view the results instantly.

## Features

- **AI Models for Virtual Try-On**: The repository includes various AI models (e.g., Eva, Rouyan, Simon, Xuanxuan, Yaqi, Yifeng) that can simulate the effect of wearing different garments.
- **Image Upload**: Users can upload their garment images (top and bottom) and a base model image for the try-on simulation.
- **Try-On Simulation**: The application processes the garment and model images and displays the resulting image where the garments are virtually "worn" by the model.
- **Pre-trained Model Support**: Easily switch between multiple AI models for different try-on styles.

## Installation

To run this project, ensure the following dependencies are installed:

```bash
pip install opencv-python numpy Pillow requests gradio
