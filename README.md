# Stability-of-Causal-Graphs

In this repository I have outlined the resouces required for conducting the experiment to check for the stability of causal graphs. 

## Data

### [Data Folder](https://github.com/Aoishi28/Stability-of-Causal-Graphs/tree/main/data)
Here you can find all the data used in this project. So for running the experiment I dropped the first three columns from the original dataset. The first two columns had the same values for all rows and the third column had unique entries for all rows. Hence the files with Copy in their name were the updated versions that were used for the project. I chose 4 datasets : ant, synapse, ivy and camel.

## Code

### [File 1](https://github.com/Aoishi28/Stability-of-Causal-Graphs/blob/main/Calculate_Jaccard_coefficient.ipynb): `Calculate_Jaccard_coefficient.ipynb`
This file is responsible for finding out the Jaccard coefficient betweeb two causal graphs. Here you just have to provide the relation between edges for the two graphs as two different inputs. Make sure that each new edge to edge relationship is in a new line. This code will output the Jaccard coefficient value.

### [File 2](https://github.com/Aoishi28/Stability-of-Causal-Graphs/blob/main/Data_generator_HOWSO.ipynb): `Data_generator_HOWSO.ipynb`
In this file, we handle data synthesis using the HOWSO algorithm. The main components include passing the files and then changing the size of the oversampled data that we want.

### [File 3](https://github.com/Aoishi28/Stability-of-Causal-Graphs/blob/main/Generate_Jaccard_Graph.ipynb): `Generate_Jaccard_Graph.ipynb`
This file's role is generating the final graph that show the distribution of Jaccard coeffcient values for each dataset.

## Steps for using Tetrad
Tetrad was used for generating the causal graphs.
To use Tetrad, do the following:
1. Step 1: [Install Tetrad](https://github.com/cmu-phil/tetrad). Use Tetrad 7.5.0-0
2. Step 2: Once Tetrad gui is installed, open a project and follow the steps mentioned in the [Tutorial](https://rawgit.com/cmu-phil/tetrad/development/tetrad-gui/src/main/resources/resources/javahelp/manual/tetrad_tutorial.html) to set up the data.
3. Select GFCI from the algorithm list and proceed to select the parameters as shown here
![image](https://github.com/Aoishi28/Stability-of-Causal-Graphs/blob/main/img/tetrad1.png)
4. Then select the combination of hyperparameters as you want
![image](https://github.com/Aoishi28/Stability-of-Causal-Graphs/blob/main/img/tetrad2.png)
6. Finally select Run Search and Generate Graph and hover select the Edges tab to copy the relationship between edges
![image](https://github.com/Aoishi28/Stability-of-Causal-Graphs/blob/main/img/tetrad3.png)
   

