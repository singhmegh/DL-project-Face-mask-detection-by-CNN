# DL-project-Face-mask-detection-by-CNN
This project detects whether a person in an image is wearing a face mask or not using a Convolutional Neural Network (CNN).
It was trained on the Face Mask Dataset from Kaggle dataset
Fetch the API from kaggle
# create a label 
with mask --> 1
without mask --> 0 

# process the image 
resize the image 
convert into array

# train test split 
make the data for train test split

# scaling the data
by min-max scaling

# building a CNN
Import tensorflow,keras
Compile the Neural network
Train the neural network

# Model evaluation
check loss and accuracy for Traing and validation data.
plot the line graph on loss and accurancy 

# make predictive model
cv2.imread() reads the image from the path.
It loads the image as a NumPy array with shape (height, width, channels) where channels are BGR (Blue-Green-Red) in OpenCV.

Shows the image inside your environment (e.g., Google Colab).
cv2.imshow() normally works on desktop Python, but in Colab we use cv2_imshow() because it’s notebook-friendly.

Resizes the image to 128×128 pixels because that’s the size your model was trained on.
Keeps 3 color channels (BGR).

Divides every pixel value by 255 to convert range 0–255 → 0–1.
Same preprocessing as you did for your training data.

Before: (128, 128, 3) → a single image
After: (1, 128, 128, 3) → a batch of 1 image (required by Keras models)
The 1 means “one image in this batch.”

if 1 then person is wearing the mass
else person is not wearing the mass

