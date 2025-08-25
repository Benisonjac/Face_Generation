# VAE Face Generator

This repository contains a TensorFlow implementation of a Variational Autoencoder (VAE) decoder for generating realistic synthetic human face images. It includes a modern web UI built with Gradio for interactive face generation.

---

## Features

- Automatically downloads and extracts the pretrained decoder model.
- Generates new face images by sampling from the learned latent space.
- User-friendly Gradio Blocks UI with styled components.
- Instant face generation by clicking a button.

---

## Getting Started

### Prerequisites

- Python 3.7 or higher
- TensorFlow
- NumPy
- Gradio
- Requests

Install dependencies with:

```bash
pip install tensorflow numpy gradio requests
```

### Usage

1. Clone this repo:
   ```bash
   git clone https://github.com/Benisonjac/vae-face-generator.git
   cd vae-face-generator
   ```

2. Run the app:
   ```bash
   python app.py
   ```

3. The pretrained VAE decoder model will download and extract automatically on first run.

4. Open the local Gradio web UI (usually at `http://localhost:7860`) and click **Generate Face** to synthesize new face images.

---

## How It Works

1. Checks if the pre-trained model file exists locally; if not, downloads and extracts it.
2. Loads the TensorFlow decoder model from the `.h5` file.
3. Samples a random latent vector from a normal distribution.
4. Runs the decoder on the latent vector to generate an image.
5. Displays generated faces in a responsive Gradio interface.

---

## Project Structure

```
├── app.py              # Main script with model loading, generation, and UI
├── requirements.txt    # Python dependencies (optional)
├── README.md           # This readme file
```

---

## Acknowledgements

- TensorFlow team for the machine learning framework.
- Gradio team for the rapid UI development library.
- Inspired by Variational Autoencoder models for generative tasks.

---

## License

This project is for educational and research purposes.

---

## Contact

For inquiries, reach out at [your-email@domain.com].
