# FRAS
Open Notebook in jupyter

Images stored in Headshots get pre-processed using open-cv and face-recognition

Resized 224x224 face images are stored in Processed_Headshots_Training, Processed_Headshots_Testing, Processed_Headshots_Validation according to 70-20-10 train-validation-test split respectively

We augment the images present in Processed_Training_Headshots and Processed_Training_Validation

Then we train the VGG16 CNN model using the Augmented folder images

We also test the model with 5 pictures not chosen for training from the facetest folder.

Run the last block to open the webcam and recognize the trained faces. Press "q" to turn off the webcam 

Detected and recognized faces from the webcam are compared with the Student_Database csv file and the corresponding student details are stored in the Attendance.csv file

Required to install these modules before running the jupyter code

pip install opencv-python
!pip install keras_vggface
!pip install keras_applications

To install facial-recognition
1. pip install cmake
2. pip install dlib

if it fails due to Python version incompatibility,
pip install dlib-19.22.99-cp39-cp39-win_amd64 

3. pip install face-recognition
