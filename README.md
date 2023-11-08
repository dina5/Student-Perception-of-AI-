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
