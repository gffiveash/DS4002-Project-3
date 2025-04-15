# DS4002 Prototyping Project 3: Flower Classification Anaylsis

## Software and Platform
- **Programming Language**: Python 3
- **Development Environment**: Google Colab
- **Libraries and Packages Used**:
  - *pandas* - for data manipulation and cleaning
  - *numpy* - numerical computation
  - *torch* -
  - *matplotlib* - for visualizations
  - *PIL* - to load image documentation
- **Platform:** Mac

## Map of Documentation

- **Data Folder**
 - **Original Data**
     - Image ID and Index.csv is a file with a unique image ID (up to 8,190) and their corresponding indexes
     - Oxford Flower Index and Name.csv is a file with flower name and its corresponding unique index number (of 102)
  - Final_Dataset.csv is our merged and cleaned CSV containing all the image, index, ID, and classification data
  - Flower Classification Data Appendix.pdf
 
- **Scripts**
  - 1_Data_Appendix.ipynb is the script to create the data appendix, highlighting key statistical summaries and visualizations
    - Output: Histogram_of_Indexes.png, Histogram_of_Flower_Types.png
  - 2_Merging_Datasets.ipynb is the script that merges the 3 individual datasets (2 in the DATA folder, 1 is the folder of 8,190 JPGs)
  - 3_EDA.ipynb is the script for EDA and visualizations, helping us understand the distribution of flower classification
    - Output: Histogram_of_Flower_Types.png, Histogram_of_Indexes.png, Top_50_Flower_Types_Bar_Graph.png

- **Output**
  - Histogram_of_Flower_Types.png
  - Histogram_of_Indexes.png
  - Top_50_Flower_Types_Bar_Graph.png
