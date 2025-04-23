# DS4002 Prototyping Project 3: Flower Classification Analysis

## Software and Platform
- **Programming Language**: Python 3
- **Development Environment**: Google Colab
- **Libraries and Packages Used**:
  - *pandas* - for data manipulation and cleaning
  - *numpy* - numerical computation
 *torch* – for building and training deep learning models using tensors and automatic differentiation  
  - *torchvision* – for accessing pre-trained models (like VGG16) and handling image transformations
  - *matplotlib* - for visualizations
  - *PIL* - to load image documentation
  - *tensorflow.keras* – for building and training the VGG16-based image classification model using transfer learning  
  - *tensorflow.keras.applications* – for importing the pre-trained VGG16 model  
  - *tensorflow.keras.preprocessing.image* – for loading and augmenting image data  
  - *tensorflow.keras.layers/models/optimizers* – for constructing the model architecture and compiling it for training

- **Platform:** Mac

## Map of Documentation
- **Data Folder**
  - **Original Data**
    - Image ID and Index.csv is a file with a unique image ID (up to 8,190) and their corresponding indexes
    - Oxford Flower Index and Name.csv is a file with flower name and its corresponding unique index number
  - Final_Dataset.csv is our merged and cleaned CSV containing all the image, index, ID, and classification data
  - Flower Classification Data Appendix.pdf
 
- **Scripts**
  - 1_Data_Appendix.ipynb is the script to create the data appendix, highlighting key statistical summaries and visualizations
    - Output: Histogram_of_Indexes.png, Histogram_of_Flower_Types.png
  - 2_Merging_Datasets.ipynb is the script that merges the 3 individual datasets (2 in the DATA folder, 1 is the folder of 8,190 JPGs)
  - 3_EDA.ipynb is the script for EDA and visualizations, helping us understand the distribution of flower classification
    - Output: Histogram_of_Flower_Types.png, Histogram_of_Indexes.png, Top_50_Flower_Types_Bar_Graph.png
 - 4_VGGmodel.ipynb is the script that builds, trains, and evaluates a CNN using transfer learning with a frozen VGG16 base to classify the 102 flower types
    - Output: Training accuracy/loss metrics, validation performance (including final accuracy), trained model ready for prediction
 

- **Output**
  - Histogram_of_Flower_Types.png
  - Histogram_of_Indexes.png
  - Top_50_Flower_Types_Bar_Graph.png
  - Epoch_Output.png
 
## Instructions for Reproducing the Results
1. Download the JPG folder of 8,000+ flower images using this link locally to your device: https://www.robots.ox.ac.uk/~vgg/data/flowers/102/102flowers.tgz.
2. Using the 2_Merging_Datasets.ipynb script to merge the 2 datasets in the DATA folder with the JPG folder.
3. Once you've merged the data and reached the finalized dataset (Final_Dataset.csv), conduct EDA using 3_EDA.ipynb in the SCRIPTS folder.
4. After you've gained an understanding of the distribution of flower classes, it is time to create our CNN model using 4_VGGmodel.ipynb in the SCRIPTS folder.
