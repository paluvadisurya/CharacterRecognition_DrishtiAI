# CharacterRecognition_DrishtiAI
Keras Deep Learning model to identify the characters present in image

![](https://i.imgur.com/BTu9wIy.jpg)

## Classification Technique
- Keras Neural Networks - Jupyter Notebook
## Dataset
- [Provided by Drishti.AI]()

### Labels
Each training and test example is assigned to one of the following labels:

| S. No | Character |
| --- | --- |
| 1 | A |
| 2 | B|
| 3 | C |
| 4 | D 

### Jupyter Notebook Index  
| S.No | Description |
| --- | --- |
| 1 | Problem Statement |
| 2 | Looking at Data   |
| 3 | Re-Sizing Images   |
| 4 | Deep Learning Model Building |
| 5 | Evaluating the Model |
| 6 | Summary
  
### Libraries Used
- Numpy
- Pandas
- Matplotlib
- Seaborn
- PIL
- Sci-Kit Learn
- Keras

---

### Procedure of Solving
1. Obtain & store the project directory location in a variable
2. Using Glob module obtain the no. of sub directories available inside our nested directory
![](https://i.imgur.com/tlf8adn.png)
3. Randomly display some images available inside the folders along with it size & label
4. If the file sizes(resolution's) are different & consists 3 layers of RGB
5. Define a function to resize all the images into a fizes square shape & convert the image data into an arra & store the image data in a variable
![](https://i.imgur.com/l4tKlAI.png)
6. Select one best rescaling method for resizing the images to make the pixels look smooth
7. Call the resizing function with our Training Data
8. Collect the labels data from the directory where the files are located & store them in a variable for target values to train the model
9. Do the same method for the testing data by collecting the information
10. Call the Independent variables & target values as X & y
11. Normalize the training data
![](https://i.imgur.com/zPeeIWF.png)
12. Split the training data into Training & Validation Data sets @20% test_size
13. Obtain the class weights for target values of training set
14. The target values are categorical in nature & convert them into one hot encoders & store the reverse lookup values in a variable.
![](https://i.imgur.com/gOpSyHp.jpg)
15. Import Keras Neural Network Library
16. Define a model function by adding Convolution 2D, Max Pooling 2D, Flatten & Dense Layers.
![](https://i.imgur.com/9sULRdw.png)
17. Call the function using our splitted training data
18. Fit the data under 20 Epochs alongside the validation data to obtain accurac score for validation data at every epoch
19. Predict the categorical classes of test images using the created model
20. Visualize the images with actual & predicted classes.
21. Print the accuracy score by evaluating the created model using test data & conclude the result.

---

### Conclusion
- Keras is one of the best library used vastly for the classification of Images
- Convolutional Neural Networks Method helped us alot to achieve a better model by adding different layers of Pooling, Flatten & Densing Laters
- The less no.of batch size denotes that model is trained properly & slowly
- Shuffling data will assure us that machine understands series of images perfectly.
- Alter the number of epochs untill we have achieved best validation accuracy & less amount of loss.
- Using Categorical Cross Entropy along side with one hot encoding provied us the best accuracy results.
- The same results can be obtained even with the Sparse_Categorical Entropy
- We have successfully obtained a model with 82% accuracy
![](https://i.imgur.com/jXcLRsy.png)
