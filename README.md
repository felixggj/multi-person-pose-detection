# Deep Learning Multi-Person Pose Detection For Sport Training Assistance
*Felix Gomez-Guillamon Jurado*

## Project Structure
- **MultiPersonPose.ipynb** - Jupyter Notebook with the code to run the model
- **requirements.yaml** - File with all the dependencies to run the project
- **README.md** - This file

## Project Description
This Deep Learning project is based on the <a href="https://tfhub.dev/google/movenet/multipose/lightning/1"> Lighting </a> Model on the
TensorFlow Hub. It will detect 17 detected keypoints on the human body and will draw the skeleton of the detected person. The model is trained on the COCO dataset. It is able to detect up to 6 people in the same video.

## Project Utilization
This model has been implemented with the aim of aiding sport coaches and trainers to detect the correct posture of their athletes. The model is able to detect up to 6 people in the same video. The model is able to detect the following keypoints:

- Nose
- Left Eye
- Right Eye
- Left Ear
- Right Ear
- Left Shoulder
- Right Shoulder
- Left Elbow
- Right Elbow
- Left Wrist
- Right Wrist
- Left Hip
- Right Hip
- Left Knee
- Right Knee
- Left Ankle
- Right Ankle

## Future Features Implementation

- Add a GUI to the interface with a Flask
- Allow users to upload a video and receive the video with the keypoints and skeleton drawn.


## Steps to run the project
### Two Options:
#### Google Colab (Using Colab's GPU)
- Install all necessary dependencies
	- Can be found on the 'requirements.yaml' file
- Upload the 'MultiPersonPose.ipynb' file to Google Colab
#### Local Computer - Silicon ARM Mac (recommended)
##### For Model Visualization
- Download <a href="https://docs.conda.io/en/main/miniconda.html">Miniconda</a>
- Create a new virtual environment with conda using 'requirements.yaml' file
	- Conda env create -f requirements.yaml
- Conda install jupyter (ignore if already installed)
- Create a specific jupyter kernel for the project for the virtual environment
	- python -m ipykernel install --user --name=ImageClassification
- Open Jupyter Lab / Notebook
