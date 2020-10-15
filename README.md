# temp_exp_normalisation
Master's Project - Normalising Temporal Expressions w/ Neural Networks

The data folder contains 4 files. The alphabet file, containing the alphabet for the word dictionaries, and the three timebank data files containing the expressions, reference dates and labels. 
The models folder contains the trained encoder and decoder models. The models were trained on 10,000 for each subcategory of temporal expression, for 10 epochs with a 
learning rate of 0.01 and with the use of teacher forcing.
The src folder contains the python notebook file containing the source code.

To run the code, open the notebook file in google colab. The alphabet data file must be uploaded to the local storage in colab found on the left-hand side pane. The models can also be uploaded there, or be stored in google drive. Wherever the models are stored, the path variables specified in the code must be altered to reflect their location. If wishing to evaluate the model on the timebank data provided, the timebank data files must also be uploaded to the colab local storage.

The TRAINING variable found at the bottom of the first cell is currently set to false, meaning when the code is run, only the validation and testing phases will be performed. To also train the model, simply set the TRAINING variable to true.

Run the code by running each cell in the notebook. The final two cells perform the model validation (on generated data) and testing (on timebank data). To test the model on different data, create and upload files in the same format as the timebank files and change the path variables in the code.
