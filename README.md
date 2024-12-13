# Cat-versus-Dog-Dataset

# Set Up Instructions
Before analyzing the code, ensure the correct modules are imported and enough stroage is available (recommended at least 2 GB).
Note the installation of the dataset may take some time depending on hardware. 
Once installed, the data does not need to be reinstalled due to recall. 

# Dependencies
The required modules are as followed to be imported:

* tensorflow (Tf) - used for training the models and is used through a majority of the dataset
* matplotlib (Plt) - used for making visualizations with the dataset
* Os - used for file pathing and creating directories
* numpy (Np) - used for array making and features

Not importing these modules will cause many problems and the code will not run. 

# Usage
Tensor flow is the most important module. To ensure it is working, the following example code can be ran to test if it was imported correctly.
import tensorflow as tf

- Check TensorFlow version (ensure it is updated!)

print("TensorFlow version:", tf.__version__)

- Creates a simple tensor and performing an operation

a = tf.constant([2, 3], dtype=tf.int32)

b = tf.constant([3, 4], dtype=tf.int32)


- Add the tensors

result = tf.add(a, b)

- Print the result

print("Result of addition:", result.numpy())

- If it is working correctly, the output should be...

TensorFlow version: 2.x.x  # Note, different versions can still work

Result of addition: [5 7]


# Data Sources
If you want to learn more about the following dataset or try your own model using the code, the page can be viewed here. 

https://www.tensorflow.org/datasets/catalog/cats_vs_dogs


If you want to learn more about tensorflow and its functions

https://www.geeksforgeeks.org/introduction-to-tensorflow/#
