# ELEVATE_LABS_DA_INTERNSHIP_DAY5_TASK5
Task 5: Exploratory Data Analysis (EDA),Objective: Extract insights using visual and statistical exploration.

DATASET USED:-https://www.kaggle.com/c/titanic/data?select=train.csv&utm_source=chatgpt.com

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

Data Preprocessing and Data Standardization(In google colab)
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


## Insights

- **Around 62% passenger died.**
- **Class 3rd was the most populated followed by 1st and then 2nd.**
- **Fare is very much right skewed.**
- **Most people bought the cheapest ticket.**
- **Shocking insight: almost more than half of the people heading for Cherbourg survived the disaster. Need to do further analysis on this point, whether this is because they are mostly from 1st class high-profile people. Need to plot a map to understand the geographic or economic point of view.**
- **Most of them are heading towards Southampton, followed by Cherbourg and Queenstown.**
- **Fare graph is very close to normal distribution, meaning less chance of having outliers. The skew and kurtosis are almost normal.**
- **Most of the people were in the age range of 20 to 40, with the highest spike at 24.**
- **Most of them were solo travelling.**
- **More males were travelling.**
- **Pclass 3 was the deadliest impacted class with the most mortality rate, while the safest option was Pclass 1.**
- **More men died than women in this disaster—almost 3/4 women survived while only 1/5 of men survived.**
- **Infants and lower age group (below 15) survived more, as saving their life was a priority. After 15 till 30, the probability of not surviving increases, then follows the path till age 33-34. Surprisingly, at 35-36, survival probability increased till 43-44, then dropped, but again rose for the age group 50 to 60; after that, no to negligible chance for surviving.**
- **Higher class people who paid more for the ticket had the most chance of surviving than those who bought cheap tickets.**
- **SibSp and Parch have high correlation, also Parch and Fare have high correlation.**
- **If someone was travelling alone, there was almost a 70% chance of not surviving. Also, with a large family size, it is less likely to survive; whereas if the family size is medium (1 to 4 members), chances of surviving are more than 56%.**

***

## Conclusion

The EDA shows a dominant gender effect: women survived at roughly three to four times the rate of men (about 74% vs 19%), making sex the single strongest observed determinant in the dataset. Class was highly stratified, with 1st‑class passengers surviving at about 63%, 2nd‑class near 47%, and 3rd‑class around 24%, reinforcing a consistent socioeconomic gradient. Embarkation patterns aligned with this gradient: Cherbourg passengers survived at about 55% compared with 39% at Queenstown and ~34% at Southampton, and the notebook flags this as a notable insight likely tied to 1st‑class mix and affluence. Family structure mattered: medium families (56% survival) fared best, while those traveling alone (30%) or in large families (15%) fared worst, suggesting benefits from limited social support without the coordination costs of large groups. Age patterns indicate children and early teens had higher survival, rates dipped through young adulthood, rose again in the mid‑30s to early‑40s, showed a smaller lift between 50–60, and fell sharply after 60, consistent with evacuation priorities and vulnerability at older ages. Fare distributions and visuals indicate survivors were concentrated at higher fares, further corroborating the class–wealth survival advantage captured by Pclass, Embarked, and Fare together. Given substantial missing Cabin data (77%) and moderate Age missing (20%), the most reliable, high‑signal features for modeling and interpretation from this EDA are Sex, Pclass, Fare, Age, Embarked, and engineered family size/type, which collectively encapsulate the study’s core patterns of advantage and risk.

***

# Thank You


