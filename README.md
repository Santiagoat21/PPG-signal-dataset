# PPG-Signal-Dataset
This dataset contains 56 records of PPG signals with a duration of 2 minutes each (fs = 100 Hz). None of the subjects were hospitalized, and data collection was carried out in a Laboratory. The data set aims to support the development of approaches to estimate blood pressure from the analysis of PPG signals.
## Data Files
This dataset is distributed in four formats:
- .csv (comma separated values).
- .mat (MatLab).
- .txt (Text file).
- .yaml (YAML ain't Markup Language).
## YAML
There are two different libraries that allow you to interact with a .yaml file in Python: pyYAML and raumel.yaml which is a fork of the previous one.

It allows you to store in a file and in a human-readable format, data that basically will be of the dictionary type (whose keys can only be strings) or lists. The values of the dictionary or list can be numeric, boolean, string, or another dictionary or list.
  
    signal: [...]             
    id: "string id"       
    age: int                 
    gender: "M or F"          
    diagnosed: "y or n"  
    treatment: "y or n"  
    sys_BP: int   
    dis_BP: int  
    HR: int   
    JNC: "N, E or H"          
    AHA: "N, E or H"
Once you have read the above file with a YAML parser, what you will have is a "normal" python dictionary.
## Information about the subjects




You can see the information about the subjects [here](https://github.com/Santiagoat21/PPG-signal-dataset/blob/775ddd4d16536d81f37f74284fe41637013963a7/information_subj.md)
