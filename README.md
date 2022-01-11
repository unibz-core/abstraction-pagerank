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
