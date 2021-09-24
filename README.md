# Master_AdvancedMachineLearning

This project's aim is the classification of fruit images from the dataset 'Fruits 360' by implementing neural networks. Tha data is contained in the zip file 'fruit-360'.

All the code was implemented through Google Colab platform and it was written in Python. 


The project is made up of different folders described as follows:
<ul>
	- Dataset.
		- fruit-360.zip: original dataset downloaded from kaggle website https://www.kaggle.com/moltean/fruits
		- multiple_fruits_label.csv: hand-crafted labels of multi-fruits dataset.

	- Images: some useful images used for the report and a video of a golden apple derived from the single-fruit dataset.

	- Models:
		- FNN_models: some FNN models implemented and saved.
		- CNN_models: some CNN models implemented and saved.

	- Notebook/Script: the code is divided in 5 Python notebooks that implement different goals, in particular:
		- 0_Exploration.ipybn: contains some initial consideration about the data as well as the visualization of some images, 
				       both before and after having applyed data augmentation. It also contains some plots that shows 
				       the labels distribution and the reconstruction of a video from which the images of a fruit were 
				       extracted (saved in the file mp4 'movie' in the Images folder).

		- 1_FNN.ipybn, 2_CNN.ipybn and 3_Fine_Tuning.ipybn: contain the implementation of the three type of neural network architectures used 
								    in this project, which are respectevely: fully connected, convolutional and convolutional 
								    with fine tuning. Each notebook shows the different models tried in order to find the optimal 
								    model. Some of those models are saved in the folders 'FNN_models' and 'CNN_models' in the Models folder.

		- 4_multiplefruits.ipybn: contains all the tests done on the multiple fruits dataset. 
					  The notebook includes the creation of the dataset with the same labels 
					  of the single fruit dataset for each image of the mulitple fruit dataset, 
					  which is saved in the csv file 'multiple_fruits_label' in the Dataset folder. 
					  The two main tests done on this dataset are the implementation of LIME 
				  	  (a type of explainable AI) and an algorithm that transforms the classifiers 					 
				  	  previously trained on single fruits into an object detector. This algorithm has 
				  	  been also implemented as a module in the python file 'ObjDetector'. It wasn't include in this repository because its size is too large.

		- ObjDetector.py: module for the object detection task.

	- Report	
		- Report.pdf: report with all explanations and comments about this project.

</ul>
