# CS171 Final Project - Classifying Animal Images
### By Anton Clayton (SJSU ID: 016358381)
#### Dataset Link: https://www.kaggle.com/datasets/alessiocorrado99/animals10

___

### Question to answer:
- "Which is harder for AI: classifying different animals or distinguishing butterfly species?"

### Our hypothesis:
- The animal model will outperform due to the distinct shapes and colors of the classes.

___

### Installation Instructions:
- No packages / modules need to be installed.
- ***___Please use Google Colab to run the notebook___***
#### There are two options for loading the dataset in Colab:
##### Option 1 (Google Drive)
1. Download the dataset zip from https://www.kaggle.com/datasets/alessiocorrado99/animals10
2. Rename zip file to "animals-dataset.zip"
3. Create a folder in your Google Drive "MyDrive" called "CS171_animals_dataset".
4. Move the "animals-dataset.zip" file to the folder
5. RUN first cell of "**Option 1**" in notebook to mount your Google Drive to colab at filepath "/content/drive/"
6. filepath to "animals-dataset.zip" should be "/content/drive/MyDrive/CS171_animals_dataset/animals-dataset.zip".
7. RUN second cell of "**Option 1**" in notebook to automatically unzip dataset zip file into path: "/content/animal_data/raw-img". After running this cell, confirm that you see **"'base_path' is set to: /content/animal_data/raw-img"**. You may also confirm by checking the "Files" directory for the new **animal_data** folder.

##### Option 2 (direct upload)
1. Download the dataset zip from https://www.kaggle.com/datasets/alessiocorrado99/animals10
2. Rename zip file to "animals-dataset.zip"
3. Upload the zip file directly to Google Colab's **content** file directory (the base file directory) such that the file path is **"/content/animals-dataset.zip"**
4. Simply run the first code cell of "**Option 2**" to automatically unzip the dataset zip file, unzipping it in the filepath: **"/content/animal_data/raw-img"**
5. To confirm that this is successful, confirm that you see **"'base_path' is set to: /content/animal_data/raw-img"**. Alternatively, you can confirm by checking the "Files" directory in Colab for the new **animal_data** folder.

#### The rest of the cells in the notebook do not have any special instructions and can be run as normal.

___

### If I were to continue this project!
If I were to continue this project, I would be really interested in exploring and expanding upon the additional hypothesis I came up with in my Notebook. I hypothesized that out of all the animals, the model would struggle the most with classifying dogs due to the vast diversity in dog breeds. Because dogs have such a wide variety of shapes, sizes, and colors, I expected the model to struggle to identify shapes and patterns in the images for dogs. Based on my analysis, it seems that I was correct. The model was the worst at classifying dogs. However, during my analysis, I found that my hypothesis could be extended further than just the intra-class variance I observed with the dog class. My model struggled more in classifying farm animals like sheep, cows, and horses while it excelled in classifying visually distinct animals like elephants and butterflies. If I were to do more for this project, I would definitely try to drop certain animals from the dataset to see how it would affect the accuracies of identifying other animals in the dataset. For example, if I dropped sheep and cows from the dataset, I would definitely expect the model's accuracy to improve for horses. With sheep and cows removed from the dataset, there are less visually similar animals to horses, making things easier for the model. To provide further evidence for my hypothesis, I was thinking of possibly adding different insects into the dataset. The model performed best on butterflies (makes sense because of their unique shape) but most of the misclassified butterflies were classified as spiders. I wonder if I add more insects into the dataset that the classification accuracy for all insects will suffer due to their visual similarities.

___

#### In my notebook, I feel that I found a good answer to our question we wanted to answer through my own dataset. Though I didn't work with Edward's butterfly dataset, I found within my own animals dataset that my model performed better on classifying visually distinct animals compared to visually similar animals.