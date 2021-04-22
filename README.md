# Table_extraction
It is a Deep Learning model for end-to-end Table detection and Tabular data extraction from Scanned Document Images

# Data source :
1. marmot dataset : https://www.icst.pku.edu.cn/cpdp/sjzy/index.htm
2. ICDAR_2017_table_dataset:https://github.com/mawanda-jun/TableTrainNet/tree/master/dataset

# Data Description:
consists of an image and its corresponding annotation which indicate the coordinate of the table present in the image. The images are in the .bmp format while the annotation file is in the .xml file.

# Brief overview TableNet Architecture:
As per the business problem statement, our input is an image file to the model, we will be getting the two outputs i.e regarding table detection and tabular structure(row and columns) identification. It is the pixel-wise detection of tabular sub-image while tabular structure recognition involves segmentation of the individual rows and columns in the detected table. The model consists of two parts which are encoder and decoder. The pre-trained VGG19 model is introduced as the baseline encoder model.

![11](https://user-images.githubusercontent.com/77537478/115711117-c6bfaa80-a390-11eb-80a4-7842e3531f03.JPG)

# Data Extraction:
After training the TableNet model and found out the best weight, one of the major tasks is to predict the table if it exists in the image and if so then extract the information from the table in the form of CSV file.

# Condition :
A High-resolution image with lots of data along with high GPU support would improved the model performance immensely.


