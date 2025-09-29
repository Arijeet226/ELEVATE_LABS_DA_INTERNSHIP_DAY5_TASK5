# ELEVATE_LABS_DA_INTERNSHIP_DAY5_TASK5
Task 5: Exploratory Data Analysis (EDA),Objective: Extract insights using visual and statistical exploration.

Titanic Dataset Analysis - Project Steps:-

Dataset Loading(In Google Collab) Loaded train dataset CSV into a pandas DataFrame.

Data Profiling(In Google Collab) Displayed initial rows of both datasets Explored dataset structure and column information Identified key columns such as survival	Survival	0 = No, 1 = Yes
pclass	Ticket class	1 = 1st, 2 = 2nd, 3 = 3rd
sex	Sex	
Age	Age in years	
sibsp	# of siblings / spouses aboard the Titanic	
parch	# of parents / children aboard the Titanic	
ticket	Ticket number	
fare	Passenger fare	
cabin	Cabin number	
embarked	Port of Embarkation	C = Cherbourg, Q = Queenstown, S = Southampton

Data Cleaning(In Google Collab) Checked for Blank Values and found out that(Cabin and age) has the most null embarked has few null.
Checked for duplicate rows and confirmed none present
Investigated missing values column-wise and calculated missing percentages
Used heatmap visualization to understand null value distribution dataset
Filled or handled missing values appropriately where needed

5. Data Preprocessing and Data Standardization(In google colab)
Changing data type for the following cols
Survived(category) PClass(category) Sex(category) Age(int) Embarked(category)
sibsp is number of siblings / spouses aboard the Titanic parch is number of parents / children aboard the Titanic as the column name length will be too lenghty so we are using the abbreviated version of it.
Ticket has numerical as well as string value so the datatype here is object.Hence, No Change.

Saved the cleaned dataset for further analysis or visualization.
![Preview](https://github.com/Arijeet226/ELEVATE_LABS_DA_INTERNSHIP_DAY5_TASK5/blob/ad68fbd87cf80657366cef4d8fde9c0f2bec195b/Screenshots/Screenshot%202025-09-29%20191049.png)

![Preview](https://github.com/Arijeet226/ELEVATE_LABS_DA_INTERNSHIP_DAY5_TASK5/blob/ad68fbd87cf80657366cef4d8fde9c0f2bec195b/Screenshots/Screenshot%202025-09-29%20191104.png)

![Preview](https://github.com/Arijeet226/ELEVATE_LABS_DA_INTERNSHIP_DAY5_TASK5/blob/ad68fbd87cf80657366cef4d8fde9c0f2bec195b/Screenshots/Screenshot%202025-09-29%20191119.png)

![Preview](https://github.com/Arijeet226/ELEVATE_LABS_DA_INTERNSHIP_DAY5_TASK5/blob/ad68fbd87cf80657366cef4d8fde9c0f2bec195b/Screenshots/Screenshot%202025-09-29%20191146.png)

![Preview](https://github.com/Arijeet226/ELEVATE_LABS_DA_INTERNSHIP_DAY5_TASK5/blob/ad68fbd87cf80657366cef4d8fde9c0f2bec195b/Screenshots/Screenshot%202025-09-29%20191135.png)

