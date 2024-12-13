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
Ensure this function runs well (may have to run previous lines of code). 
Once working, every run will result in a different image (can either be cat or dog).

def rand_image(dataset):
my_image = dataset.take(1) # retrieves the first sample from a random class

for image, label in my_image:
  
  img = image[0]
  
  label = label[0]

  index = np.argmax(label)

  if index == 0:
    label = 'cat'
  else:
    label = 'dog'

  plt.imshow(img)
  plt.title(label)
  plt.axis("off")

# Data Sources
If you want to learn more about the following dataset or try your own model using the code, the page can be viewed here. 

https://www.tensorflow.org/datasets/catalog/cats_vs_dogs
