# BME3053C_FinalProject_TrifectaTech

Our program was split into multiple individual, smaller prpgrams that all help accomplish our solution. 
The code is posted here without the data. Each program builds off of the last one, using the output of one program as the input of the next, etc.

The Project_Data_Extraction file takes the raw data, which is in a timeseries format, and extracts it, putting it into a matrix

The From_Label_To_Vector file extracts the sleep stage data from the text data, putting it into a matrix that can be used by later programs

The Project_Matrix_Creator file combines the data extracted from the previous two programs into a single matrix with a format that can be used in the next step

The From_Mat_to_Model file takes the matrix and runs it through an LDA model to create a machine learning to predict sleep stages of data that can be input
into the model; it then computes its accuracy of predicting sleep stages

The Patient_Sleep_Stages file looks at individual patients and determines the amount of time the patient spent in each sleep stage by putting data from
past steps into the Stage_Hours file, which is a function
