# CA-Markov program for Land Use Land Cover Classification with GeoAI
This project is designed to predict future Land Use Land Cover Classification (LULC) changes from available data using a combination of Cellular Automata (CA) and Markov chain.
## Setup
-  Prerequisites: Python 3.7+, Python PIP installer, Jupyter notebook, Aligned LULC Classified images of a particular region seperated by equal time interval
- Required python packages (PIL, NumPy, Pydrive, tabulate) can be installed with Python PIP
- The location of the images needs to be set in the program
## Execution
- Images seperated by equal time interval, say T years, provide training dataset to generate matrix
- New image can be taken as test for prediction
- In CA predict, there is an option to choose mode of prediction
- For mode 0, only maximum probability of change is always selected
- For mode 1, random number is used to assign prediction values so that all probabilties are considered
- Program takes around 40-50 minutes to generate output
- Output file will be generated in BMP format, stored in the same folder as the code and will contain prediction on test image for T years in future
- Eg. If 2005, 2010 and 2015 are given as trining dataset and 2000 image is given for test, we can get prediction for year 2005 as output
- A comparison table is added with output to display in test image and predicted image
