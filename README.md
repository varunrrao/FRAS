# FRAS
Open Notebook in jupyter

Images stored in Headshots get pre processed and the resized face images are stored in Processed_Headshots

Then we train the vgg16 cnn model using the Processed_Headshots folder images

We also test the model with 5 pictures not chosen for training from the facetest folder.

Run the last block to open webcam and recognize the trained faces. Press "q" to turn off the webcam 

Required to install these modules before running the jupyter code

pip install opencv-python
!pip install keras_vggface
!pip install keras_applications

To install facial-recognition
1. pip install cmake
2. pip install dlib

if it fails due to python version incompatibility,
pip install dlib-19.22.99-cp39-cp39-win_amd64 

3. pip install face-recognition
