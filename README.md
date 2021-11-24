# MNIST-Neural-Network
My first neural network that detect handwritten numbers from webcam images. Trained on MNIST dataset.

I made this on google collab and so if you want to try the webcam image detection you can check this: https://colab.research.google.com/drive/1OdHG7pLl3pIMusysF5Rmke0KnoP_ezmz?usp=sharing

I did not know how to code the webcam implementation part but stumbled upon a tutorial by Anmol Chawla on Youtube and so the image capturing part is implemented using code from his GitHub: https://github.com/anmolchawla/MNSIT-Webcam-Tutorial

Note:
There was a ValueError in the prediction of the image captured but I fixed it by adding

user_test=user_test.reshape(-1,img_size,img_size)

after

user_test = tf.keras.utils.normalize(new_array, axis = 1)
