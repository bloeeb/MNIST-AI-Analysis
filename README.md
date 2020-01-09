# MNIST-AI-Analysis

The MNIST analysis was the final project of my tensorflow online course (Deep Learning with Tensorflow 2.0) and a good first Github project.
I will give a short overview here, but most of my thoughts are already written as comments in the code.

As the MNIST dataset is included in the tensorflow_datasets library it can easily be used as a first practicing project using TF.
After importing the relevant libraries and loading the dataset a first important step was splitting the data into a train, validation and test batch. A 80-10-10 split was used.
Another important step was scaling the data. The MNIST dataset includes ~70k handwritten pictures of numbers between 0-9. For the computer these pictures are 28x28 big pixel squares with values between 0-255 (0 being black and 255 being white). With scaling these numbers are put on a numerically more stable basis between 0 and 1.
Next the dataset was shuffled. This is especially important for datasets where there might be a danger of sorting such as according to dates or in our case numbers. If we don't sort all 8s might be in the validation batch. To even the dataset out it is hence shuffled.
Afterwards the model was created. After some testing I came to the conclusion that two hidden layers were enough, additional ones did not bring any improvement in accuracy. 
After training the model and testing it against the test set an accuracy of ~ 97.8% could be reached.
That means that the algorithm is able to classify the image of a handwritten number with a chance of 97.8% correctly. I want to try to further improve this number in the future, with additional knowledge that I will gain while getting more into the topic.

As this was one of the final projects of the course it was heavily guided by the course leader. Nevertheless, I learned a lot in the process and want to try using this new knowledge to create some own AI projects in the future. Tips and critique are very welcome! Thanks for reading
