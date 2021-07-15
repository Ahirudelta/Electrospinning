# Electrospinning
This is the python code and data of the senior project of Teeruch Sintusiri
In the topic Modeling and optimization of electrospinning parameters for prediction the nanofiber diameter by using artifitial neural network.

Information of each folder
- original
  - The data of each material is contain in this folder.
  - The data must be the .csv file.
  - The data must contain 4 parameters including:
    - Concentration -> con
    - Aplied voltage (kV) -> vol
    - Tip to collector distance (cm) -> dis
    - Feed rate (mL/hr) -> feed
 - norm_file
    - This folder contain the normalization of each dataset from the original folder.
    - The normalize formula is x_norm = x/(x_max - x_min)
    - Have to add "norm_" to the columns name
 - error_table
    - This folder contain the error value of each model.
    - Typically, file in this folder created by running the training process.
 - test_train
    - This folder contain the testing and training dataset which splited while trainning process.
 - The folder which start with "model"
    - This kind of folder created for collect the ANN model while training process.
    - In the folder, have to create the folder named "loss" for collect the loss of each model.


Python code
  - Train_model.ipynb
  - Predict_and_plot.ipynb
  - R2_evaluate.ipynb
