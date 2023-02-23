# Installation & Running

- Download Zip Folder Py_Files (Unzip)

- Files Structure

          2 Folders & 5 .py files
        - Support_Data
            - tasks.xlsx
            - cost.csv
            - suppliers.csv

        - Figures (Automatically gets created after execution of Acme Python)
            - SectionNo_Image.png (Starts saving after succesful exceution of Acme Python)

        - Step1_DataPreprocessing.py
        - Step2_EDA.py
        - Step3_ModelFitting.py
        - Step4_RMSE.py
        - Step5_CV_&_HPO.py (Cross Validation and Hyper-parameter Optimization)
        - main.py
        
        - BeePy Presentation.pdf
        - BeePy.ipynb
    
- Dependencies required / Installation

        - Open terminal/cmd/Code Editor(Spyder/ PyCharm)
        - python 3.7 + (respective pip version) / stable conda
        - standard packages like numpy, pandas are added in top of the .py files
        - section specific packages are included in different section
        - all those packages are necessary to run the code smoothly
                -  Method 1 )   pip/conda install package name is needed to 
                                - Dependencies needed :
                                - pandas, numpy, copy, 
                                - os, dataframe_image, sklearn, 
                                - matplotlib, seaborn, natsort, 
                                - plotly, random, etc.
                                - Some dependencies/packages require specific versions of python, pip, pandas, numpy combination,
                          hence, kindly use the stable versions
        - requirements.txt has the versions included for different packages
        - In Terminal/Cmd run > pip/conda install -r requirements.txt

- Running Python File

        - Move to respective directory in cmd/terminal/code editor 
          ex - cd "Downloads/python_BeePy/Py_Files" 

        - In terminal/cmd run > python Step5_CV_&_HPO.py
        - Or run >python main.py
        - Step 5 includes all the previous steps imported
        - Individual steps can also run individually

# Brief: 
The Acme Corporation must complete a task every day; these can be e.g. deliveries of goods,
project management tasks, or recruitment of staff. For completing each task, Acme must choose one
out of sixty-four (64) suppliers that provide the resources required to complete the task. The final cost
of the task depends on how effective the chosen supplier is at performing the particular task.
Unfortunately, estimating this cost in advance requires significant resources. Acme has hired your
Business Analytics firm to develop a machine learning (ML) approach for selecting suppliers given a
new task.

To complete your assignment, Acme has provided you with three datasets:

 ‘tasks.xlsx’: an Excel file that contains one row per task and one column per task feature
(TF1, TF2, TF3, …, T116). Each task is uniquely identified by a Task ID (a date, eg., ‘2019 05
30’).

 ‘suppliers.csv’: A CSV file that contains one row per supplier and one column per supplier
feature (SF1, SF2, …, SF18). Each supplier is uniquely identified by a Supplier ID given in the
first column of the file (S1, …, S64).

 ‘costs.csv’: a CSV file that contains data collected and/or estimated by Acme about the cost
of a task when performed by each supplier. Each row gives the cost value (in millions of dollars,
M$) of one task performed by one supplier.

Your goal is to provide Acme with an ML model that, given the task features of a task, selects one
supplier among the 64 suppliers available. 
