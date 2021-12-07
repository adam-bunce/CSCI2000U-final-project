## What Drives Student Success In Math and Language Courses

## About Us
Adam Bunce     &nbsp;  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  - [adam-bunce](https://github.com/adam-bunce)<br>
Addison Tung  &nbsp;  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp; - [Elucris]( https://github.com/Elucris) <br>
Santhosh Chelvaranjan &nbsp; - [SanthoshC8]( https://github.com/SanthoshC8)<br>


## Introduction
What makes a student successful? Is it how long they study? How frequently do they skip school? Or is it just based on how naturally gifted they are. To answer these questions, we used a [Kaggle Dataset](https://www.kaggle.com/uciml/student-alcohol-consumption) that consists of 395 secondary student's scores in math and Portuguese language courses obtained through a survey. Along with this we are given information about the student's; age, sex, internet access, drinking habits, family situation, study habits and several other features.     





## Discussion 
Let's start off with some questions to further analyse:
1. What are the key factors that contribute to a student's performance? Do any key features particularly stand out?
2. Do any features out of the students control have a negative impact on their performance?
3. Since our dataset includes the students alcohol consumption, does the level of consumption affect the students ability to excel in their class? Are there external factors that contribute to the level of consumption?

At an initial glance, the best way to parse through a dataset this large is through the use of a correlation matrix. Here we used a heatmap to emphasize any possible trends shown below

![image](https://user-images.githubusercontent.com/74341873/144947713-6b993f2e-f4cc-4da1-9ad2-0a6639857546.png)

What are the notable features we can identify in this graph? Here we can see strong correlations between the first class, second class, and final grades where students performing well will excel throughout the entire class. There is also a strong trend with a student's freetime, going out, and their alcohol consumption which is reasonable enough as going out typically implies having a good time.

Looking at the more negative side of this graph, we see connections between the number of failures in the class and a student's final grades where if one fails they are more likely to fail again. This trend also relates to the students' age.

Let's take a look at parental influence in our dataset while also checking their absences in the class. We are checking both parents' level of education and seeing if that plays a role in the student’s performance.


![image](https://user-images.githubusercontent.com/74341873/144949542-07d7b5bb-d7ab-41c6-8a97-447d5b896c19.png)

![image](https://user-images.githubusercontent.com/74341873/144949552-c02e0227-9622-4906-b4d4-6bbeac2b9e0f.png)


Here we can see a general positive trend in the parents' education level and their student’s performance. However it is clear that the mother has more influence over the father when it comes to the students' education.


Does extra educational support affect grades? Surprisingly not. Infact, the average grade of students with no extra help was higher than the students who did have help. There could be a few reasons why this happened. The students that were confident in their studies are less likely to ask for extra help. While the students struggling in class would look for more educational support. Clearly even with the extra help, students aren’t able to improve their grades.

![image](https://user-images.githubusercontent.com/74341873/144948299-2dd21d13-b0fe-49f5-b0e5-9c3095ddc38f.png)

![image](https://user-images.githubusercontent.com/74341873/144948464-90cade49-b2ce-40ee-9cb7-6a526dd456ae.png)


Even the students that pay for extra classes didn’t have an advantage over the students who didn’t. The students with the highest grade didn’t have any paid extra classes. 
Clearly, having additional support/classes does not affect grades as much as one would expect.




Do students drinking alcohol affect grades? Yes. Generally, the less you drink alcohol, the higher your grades will be. 

![image](https://user-images.githubusercontent.com/74341873/144948365-8380023e-0128-47ef-8cb7-904440151308.png)


It was surprising that the average grade of students with a very high alcohol consumption was equal to those with a low alcohol consumption during workdays. The students with the highest grades also drank no alcohol during workdays. 

![image](https://user-images.githubusercontent.com/74341873/144948551-4a42e0a1-d406-4654-a2d4-155490974e6c.png)



Students who didn’t drink much alcohol during weekends had a higher average than those who drank a lot. The students with the highest grades also drank the least during weekends.



## Conclusion
<b>Reflection: </b><br>
Generally having educated parents, drinking less alcohol, and attending more classes are all ways to improve your success as a student.
Features that most increase students’ success are mothers' education level and hours they spent studying. 
Features that most decrease students’ success are travel time, number of classes they have failed before, and the frequency with which they go out.



<b>Refinement:</b> <br>
If we were to improve the project, we could have chosen a better dataset that had more students surveyed. You would get more accurate results on what influences grades if more students were polled instead of just the ~400 in the current dataset. 
We could also compare features to first and second period grades instead of only G3.


## Acknowledgements

This project was submitted as the final course project for CSCI 2000U “Scientific 
Data Analysis” during Fall 2021. The authors certify that the work in this 
repository is original.

# README
<b>Installation:</b><br>
Run on any linux distribution, was compiled on Ubuntu 20.04.<br>
Clone to your machine to work with this repository.
<pre>$ git clone https://github.com/adam-bunce/CSCI2000U-final-project </pre>

<b>Requirements:</b><br>
Python 3.8.2 or newer <br>
seaborn               <br>
NumPy                 <br>
pandas                <br>
Matplotlib            <br>
scikit-learn          <br>

<b>Usage:</b><br>
Having both student-por.csv and student-math.cvs in the root folder and dependencies installed open CSCI2000U-final-project.ipynb and select ![image](https://user-images.githubusercontent.com/74341873/144947949-23c87493-d001-4b36-866e-bbe8327f7e52.png) at the top of the notebook to run the whole notebook.
