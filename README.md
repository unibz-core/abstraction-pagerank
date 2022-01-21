# abstraction-pagerank
Notebook to run a conceptual model abstraction algorithm.
This algorithm is based on Google Page Rank folowing the paper:

Huang, Liang, et al. "Enhancing UML Class Diagram Abstraction with Page Rank Algorithm and Relationship Abstraction Rules." International Conference on Service-Oriented Computing. Springer, Cham, 2016.

This algorithm implementation is part of a comparative analysis between differente conceptual model abstraction approaches. 

Contributors:

* Guylerme Figueiredo (UFES)

## Requirements
There is no specific requirements to run this algorithm. This is a notebook that can be ran on Google Colaboratory or any other notebook tool.

The dependencies is loaded on the source code.

## Usage
Basically this notebook needs two parameters to run. The first one is the model, exported from a OntoUML model in JSON format. This model was exported using Visual Paradigm with OntoUML plug-in.
In command 4 the notebook will ask to upload JSON file.

The second param is the diagram name. The model can contain various diagrams, so we need to inform which diagram will be considere to run the algorithm. You inform this param on command 6.

After inform the two parameters you can run all others commands to generate the result of conceptual model abstraction.

At the end of algorithm we generate two csv files: one containing the classes and the other file containing the relations os abstracted conceptual model.

## Step by Step

This code can be used in any notebook tool, such as Jupiter Notebook, Databricks, etc.

In our case, we implemented it using Google's Colab tool.

To run the algorithm and obtain the resulting model using PageRank just follow the steps below:

1- When you access the code "Abstraction_PageRank_Final.ipynb" through the GitHub link (https://github.com/unibz-core/abstraction-pagerank/blob/main/Abstraction_PageRank_Final.ipynb), you will see a button right at the beginning of the code to open this same code in Google Colab (Open in Colab)

2- When in Colab, each cell corresponds to a command that can be run independently, but for the algorithm to execute correctly, the cells must be executed in order. Thus, in this step you will go to cell 6 and next to it inform the name of the diagram. The diagram name is the one you will use as a reference from the model you are going to upload.

3- On the Google Colab menu bar, click Runtime --> Run all

4- Next to each cell, the icon will indicate if the command is being executed or if it has already been executed. If it has a green tick, the command was successfully executed.

5- You will notice that cell 4 will inform that it was executed, but cell 5 will keep signaling that it is being executed. At this point, notice that a button will appear just below cell 5 for you to upload the file. At this point, click the button and upload the exported model in JSON.

6- Now is to wait for all the commands to execute. This should take a little over 20 minutes.

7- At the end, on the left bar there is a folder icon. When you click on the link you will notice that you have two resulting files "classes.csv" and "relation.csv" which is the list of elements that will compose the abstracted model.
