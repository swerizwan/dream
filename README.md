# DREAM: Deep 3D Facial Reconstruction for Emotion Analysis and Modeling

## About the Project

DREAM (Deep 3D Facial Reconstruction for Emotion-Aware Health Monitoring) enhances parametric 3D face model reconstruction to capture nuanced emotional expressions. By integrating emotional detail encoding and decoding with FLAME and Render modules, the project synthesizes realistic 3D facial expressions. Training with deep perceptual emotion analysis improves expression fidelity, surpassing baseline techniques and demonstrating efficacy in health monitoring applications.

## Installation

1. **Clone the Repository**: Download the project from GitHub.
2. **Set Up Conda Environment**: Create a Conda environment named DREAM with Python 3.9:
    ```bash
    conda create --name dream python=3.9
    conda activate dream
    conda install mamba -n base -c conda-forge
    ```
3. **Install Dependencies**: Install the required packages using pip:
    ```bash
    pip install -r requirements.txt
    ```

## Datasets

The project utilizes three diverse datasets:

- **IEMOCAP Dataset**: Annotated with categorical labels like happiness, sadness, anger, and neutral, it offers ten hours of audio and video recordings from spontaneous sessions between actors. [IEMOCAP Dataset](https://sail.usc.edu/iemocap/iemocap_release.htm)
- **AffectNet Dataset**: With over one million facial images annotated with seven primary emotions, it provides a rich resource for emotion recognition research. [AffectNet Dataset](http://mohammadmahoor.com/affectnet/)
- **CMU-MOSEI Dataset**: Annotated with continuous emotion dimensions like valence and arousal, it includes multimodal data suitable for emotion recognition and sentiment analysis tasks. [CMU-MOSEI Dataset](http://multicomp.cs.cmu.edu/resources/cmu-mosi-dataset/)

## Steps for Training

1. **Download Dataset**: Download the dataset from the provided links.
2. **Data Processing**: Run the `process_data.py` script to preprocess the dataset.
3. **Initiate Training**: Execute `python training/train_dream.py` to begin the training process.

## Running the Demo

Follow these steps to run the demo of the project:

1. **Download Pre-trained Models**: Obtain the pre-trained DREAM model and FLAME model from the provided links.
2. **Demo for Images**: Run `python dream_image.py` for processing images.
3. **Demo for Videos**: Run `python dream_video.py` for processing videos.
