# PPG-Signal-Dataset
This dataset contains 56 records of PPG signals with a duration of 2 minutes each (fs = 100 Hz). None of the subjects were hospitalized, and data collection was carried out in a Laboratory. The data set aims to support the development of approaches to estimate blood pressure from the analysis of PPG signals.
## Data Files
This dataset is distributed in four formats:
- .csv (comma separated values).
- .mat (MatLab).
- .txt (Text file).
- .yaml (YAML ain't Markup Language).
### YAML
There are two different libraries that allow you to interact with a .yaml file in Python: pyYAML and raumel.yaml which is a fork of the previous one.

It allows you to store in a file and in a human-readable format, data that basically will be of the dictionary type (whose keys can only be strings) or lists. The values of the dictionary or list can be numeric, boolean, string, or another dictionary or list.
  
    - signal: [...]               # Placeholder for signal data, likely an array
    - record: "string record"     # Unique identifier for each record (string type)
    - age: int                    # Age of the subject (integer type)
    - gender: "M or F"            # Gender of the subject (M for male, F for female)
    - diagnosed: "y or n"         # Indicates if the subject has been diagnosed (y for yes, n for no)
    - treatment: "y or n"         # Indicates if the subject is under treatment (y for yes, n for no)
    - systolic_BP: int            # Systolic blood pressure of the subject (integer type)
    - distolic_BP: int            # Diastolic blood pressure of the subject (integer type)
    - HR: int                     # Heart rate of the subject (integer type)
    - JNC: "N, E or H"            # Blood pressure classification by JNC (N for normal, E for elevated, H for hypertension)
    - AHA: "N, E or H"            # Blood pressure classification by AHA (N for normal, E for elevated, H for hypertension)


Once you have read the above file with a YAML parser, what you will have is a "normal" python dictionary.
## Information about the subjects
The table presents detailed information on various health metrics for 56 subjects:

- **Gender**: Indicates the gender of the subject (M for male, F for female).
- **Treatment**: A binary indicator (y for yes, n for no) specifying whether the subject is currently undergoing medical treatment.
- **Systolic Blood Pressure (Systolic BP)**: Represents the systolic blood pressure of the subject.
- **Diastolic Blood Pressure (Diastolic BP)**: Indicates the diastolic blood pressure of the subject.
- **Heart Rate**: Shows the heart rate of the subject.

Additionally, each subject is uniquely identified by a record number, and the average age across all subjects is approximately 52.48 years, with a standard deviation of about 7.16 years. The age range spans from a minimum of 44 years to a maximum of 65 years. The columns labeled “JNC” and “AHA” provide classifications of blood pressure according to the Eighth Joint National Committee and the American Heart Association, respectively.


You can see the information about the subjects [here](https://github.com/Santiagoat21/PPG-signal-dataset/blob/775ddd4d16536d81f37f74284fe41637013963a7/information_subj.md)
## Made by
- Erick Javier Arguello - erick.arguello00@usc.edu.co (Collaborator)
- Werner Gordon Uribe - werner.gordon00@usc.edu.co
- Santiago Escobar Manrique - santiago.escobar01@usc.edu.co

##References
1. Como crear y leer archivos yaml en python? (s. f.). Stack Overflow En Español. https://es.stackoverflow.com/questions/151852/como-crear-y-leer-archivos-yaml-en-python
2. Chobanian, A. V., Bakris, G. L., Black, H. R., Cushman, W. C., Green, L. A., Izzo Jr, J. L., ... & National High Blood Pressure Education Program Coordinating Committee. (2003). Seventh report of the joint national committee on prevention, detection, evaluation, and treatment of high blood pressure. hypertension, 42(6), 1206-1252.
