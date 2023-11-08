# Student-Perception-of-AI-

### Abstract 
This is a personal research project that focuses on the relationship between AI and students in an educational setting, with a particular emphasis on HCI principles in educational AI systems. This project explores students' knowledge levels and attitudes toward AI. Although the analysis is ongoing, it has already uncovered several key insights. Most students have AI knowledge ratings between 4 and 8, with the internet being their main source of AI-related information. The majority of students hold either optimistic or pessimistic views toward AI, with those having higher AI knowledge ratings tending to have more positive opinions. A significant number of students express curiosity about AI, indicating a growing interest in the field. Students predict medicine will be most impacted by AI, while art will be least affected. Additionally, AI knowledge ratings are correlated with utility grading, with female third-year students in statistics and economic forecasting having a higher representation in the survey, while male students had lower exam pass rates. Finally, there is a weak correlation between AI knowledge ratings and GPA.

# Dataset Information
Thisn is a part of a suervey data and it is obtained from Kaggle. The size may be somewhat small and there may be a selection bias via who answered the survey there is still value to be gained within these limitations.

# Tools & Technology
- Python programming language
- Google colab
- Pandas, numpy, matplotlib and seaborn

# Configuration
If you want to run directly using API command, then apply the following procedures: <br>

STEP 1: Install kaggle
~~~
!pip install kaggle
~~~

STEP 2: Update with kaggle.json file
~~~
from google.colab import files
files.upload()
~~~

STEP 3: Move the uploaded "kaggle.json" file to the correct location. Run the following command in a code cell:
~~~
!mkdir ~/.kaggle
!cp kaggle.json ~/.kaggle/
~~~

STEP 4: Set the appropriate permissions
~~~
!chmod 600 ~/.kaggle/kaggle.json
~~~

STEP 5: Now unzip the dataset
~~~
!unzip survey-on-students-perceptions-of-ai-in-education
~~~

# First few columns of the dataset

| ID | Q1.AI_knowledge | Q2.AI_sources | Q2#1.Internet | Q2#2.Books/Papers | Q2#3.Social_media | Q2#4.Discussions | Q2#5.NotInformed | Q3#1.AI_dehumanization | Q3#2.Job_replacement | ... | Q7.Utility_grade | Q8.Advantage_teaching | Q9.Advantage_learning | Q10.Advantage_evaluation | Q11.Disadvantage_educational_process | Q12.Gender | Q13.Year_of_study | Q14.Major | Q15.Passed_exams | Q16.GPA |
|----|-----------------|--------------|--------------|------------------|-----------------|-----------------|------------------|-----------------------|-------------------|-----|-----------------|-----------------------|----------------------|------------------------|----------------------------------|----------|-----------------|----------|-----------------|-------|
| 0  | 1             | 8            | Internet     | Books/Scientific papers (physical/online) | 1 | 1 | 0 | 0 | 1 | 2 | ... | 9 | 3 | 1 | 2 | 3 | 1 | 2 | 2 | 1 | 9.2 |
| 1  | 2             | 7            | Internet; Social media | 1 | 0 | 1 | 0 | 0 | 2 | 3 | ... | 6 | 2 | 2 | 1 | 2 | 2 | 2 | 2 | 1 | 7.7 |
| 2  | 3             | 5            | Internet; Books/Scientific papers (physical/online) | 1 | 1 | 0 | 0 | 0 | 2 | 1 | ... | 6 | 3 | 3 | 3 | 4 | 2 | 2 | 2 | 0 | 7.2 |



