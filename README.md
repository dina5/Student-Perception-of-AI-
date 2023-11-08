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

# First three rows of the dataset

| ID | Q1.AI_knowledge | Q2.AI_sources | Q2#1.Internet | Q2#2.Books/Papers | Q2#3.Social_media | Q2#4.Discussions | Q2#5.NotInformed | Q3#1.AI_dehumanization | Q3#2.Job_replacement | ... | Q7.Utility_grade | Q8.Advantage_teaching | Q9.Advantage_learning | Q10.Advantage_evaluation | Q11.Disadvantage_educational_process | Q12.Gender | Q13.Year_of_study | Q14.Major | Q15.Passed_exams | Q16.GPA |
|----|-----------------|--------------|--------------|------------------|-----------------|-----------------|------------------|-----------------------|-------------------|-----|-----------------|-----------------------|----------------------|------------------------|----------------------------------|----------|-----------------|----------|-----------------|-------|
| 0  | 1             | 8            | Internet     | Books/Scientific papers (physical/online) | 1 | 1 | 0 | 0 | 1 | 2 | ... | 9 | 3 | 1 | 2 | 3 | 1 | 2 | 2 | 1 | 9.2 |
| 1  | 2             | 7            | Internet; Social media | 1 | 0 | 1 | 0 | 0 | 2 | 3 | ... | 6 | 2 | 2 | 1 | 2 | 2 | 2 | 2 | 1 | 7.7 |
| 2  | 3             | 5            | Internet; Books/Scientific papers (physical/online) | 1 | 1 | 0 | 0 | 0 | 2 | 1 | ... | 6 | 3 | 3 | 3 | 4 | 2 | 2 | 2 | 0 | 7.2 |


# Exploratory data analysis based on the survey questions

To analyze the dataset, I have just explained a few questions. Let's explore:

## Question 1

On a scale of 1 to 10, how informed do you think you are about the concept of artificial intelligence? <br>

The first thing we would like to know is what is the general distribution of how informed people think they are. This can be done using a seaborn countplot - using the dataframe df and x is the name of the Q1 column. I have used a red color for the bars to ensure consistency across the graphs.

![download](https://github.com/dina5/Student-Perception-of-AI-/assets/24854710/c3a18989-226f-470c-944a-d5765fe3d11e)

**Insight:** The results of the first question seem to form a bell curve with most students having a confidence of 5 to 7 and some outliers who have a confidence of 1, 2, 3, or 10. We can explore more about some of the students that fall in these ranges in more detail later.

## Question 2

What sources do you use to learn about the concept of artificial intelligence?
- Internet
- Books/Scientific Papers
- Social Media
- Discussions
- "I don't inform myself about AI"
  
Some things that would be interesting to know would be what proportion of the students use each source (2i), is there any correlation between the sources used (2ii) and how is a student's ai knowledge rating related to their sources of information (2iii)

![002](https://github.com/dina5/Student-Perception-of-AI-/assets/24854710/b165399a-3454-4d54-8e8a-c8bb1db1f427)

**Insight:** We can see visually that the internet is by far the most commonly used source of information. this makes sense as a internet contains a huge library of available of information. Very few students claimed to be uninformed so hopefully that is a positive step in the right direction.

# Overall Findings

Although this is an incomplete analysis, there have been many interesting insights that have been found. These include:

1. Most students had an AI knowledge rating between 4 and 8.
2. The internet is the most common source of information.
3. There are mainly two groups of attitudes towards AI:
   - Students who think AI will solve problems and boost the economy.
   - Students who think AI will reduce the number of opportunities for humans, including jobs.
4. Increased AI knowledge rating tended to have more positive opinions.
5. Most students are curious about AI.
6. Students think that medicine will be the domain that sees the largest impact from AI.
7. Students think art will see the smallest impact from AI.
8. AI knowledge rating is correlated with utility grading.
9. Female year 3 students in stats and economic forecasting had the highest representation in the survey.
10. Male students included in the survey tended to have significantly lower rates of passing all their exams.
11. There is a weak correlation between AI knowledge rating and GPA.

These findings provide valuable insights into the perceptions and attitudes of students towards artificial intelligence.


