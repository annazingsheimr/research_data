# research_data
Research data associated with article Optimal Design and Operation of an Integrated Wind, Electricity, Hydrogen, and Electro Fuel System with Storage to Decarbonise Iceland

This research data repository is structured into three main folders: Data, Model, and Results. All data, except hourly electricity consumption data by regional zone in Iceland which is subject to a non-disclosure agreement (NDA) with the Transmission System Operator of Iceland, and all code used to work the data is shown in the Data folder. The model code for both scenarios is shown in the Model folder, while the Results folder presents the output results for each scenario and all the code necessary to reproduce graphs, figures, and other results presented in the article. 

All python code files use and input and an output. Where the input is not directly inserted into the code but uploaded via a file, a filepath is to the input data is used. A filepath is also used to locate the output data. These filepaths will present the data repository structure, but should be adjusted to the user's needs after dowloading the data and code files.

Data
The Data folder contains six folders: aviation, electricity, hydrogen, maritime, technoeconomics, and wind. Its purpose is to provide the code to produce the datasets and the datasets itself to be used in the model (in the Model folder). The aviation, hydrogen, and maritime folder all contain a PY file with code to produce the dataset that is also in the respective folders. The electricity file only contains the code and not the hourly electricity consumption input, as the hourly electricity consumption data for each zone in Iceland from several years is subject to an NDA, and thus the final dataset cannot be provided. However, users can produce their own datasets using the code; you would simply need an hourly electricity consumption dataset (for different zones). The maritime folder shows three code files and three output files; the shipping_demand.py and fishind_demand.py produce the datasets (fishing_demand.csv and shipping_demand.csv) which are then used as inputs in the fishing_shipping.py file to produce the maritime_demand.csv dataset (for use in the model). The maritime folder also contains löndunarhafnir.xlsx, which is used to allocate individual ports in Iceland to the correct zone as defined by the boundaries in the research paper. All technoeconomic data is put directly into the parameter python files (located in the Model folder), according to the Methodology & Data section in the research paper and in line with the sources referenced there. 
The wind folder contains two code files and several input folders/files.

Model 

Results
