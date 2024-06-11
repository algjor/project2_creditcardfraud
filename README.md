
# PROJECT #2:  PREDICTION OF DIVORCE

# Problem Statement
Problem Statement: To investigate the correlation between the individual questions and their influence on marriage retention.
Objective: To predict the likelihood of couples staying together or getting a divorce.

# Background

The dataset that we selected for this project was Predicting Divorce dataset (divorce.csv") from Kaggle.
This original data set was comprised originally of 55 questions that were asked to 170 couples. Answers to certain questions were used to detemine if a couple is likely to get divorced in the future.
The questions are ranked on a scale of 1-4 with 1 being the lowest and 4 being the highest. The last category states if the couple has divorced.
1.  If one of us apologizes when our discussion deteriorates, the discussion ends.
2.  I know we can ignore our differences, even if things get hard sometimes.
3.  When we need it, we can take our discussions with my spouse from the beginning and correct it.
4.  When I discuss with my spouse, to contact him will eventually work.
5.  The time I spent with my wife is special for us.
6.  We don't have time at home as partners.
7.  We are like two strangers who share the same environment at home rather than family.
8.  I enjoy our holidays with my wife.
9.  I enjoy traveling with my wife.
10. Most of our goals are common to my spouse.
11. I think that one day in the future, when I look back, I see that my spouse and I have been in harmony with each other.
12. My spouse and I have similar values in terms of personal freedom.
13. My spouse and I have similar sense of entertainment.
14. Most of our goals for people (children, friends, etc.) are the same.
15. Our dreams with my spouse are similar and harmonious.
16. We're compatible with my spouse about what love should be.
17. We share the same views about being happy in our life with my spouse
18. My spouse and I have similar ideas about how marriage should be
19. My spouse and I have similar ideas about how roles should be in marriage
20. My spouse and I have similar values in trust.
21. I know exactly what my wife likes.
22. I know how my spouse wants to be taken care of when she/he sick.
23. I know my spouse's favorite food.
24. I can tell you what kind of stress my spouse is facing in her/his life.
25. I have knowledge of my spouse's inner world.
26. I know my spouse's basic anxieties.
27. I know what my spouse's current sources of stress are.
28. I know my spouse's hopes and wishes.
29. I know my spouse very well.
30. I know my spouse's friends and their social relationships.
31. I feel aggressive when I argue with my spouse.
32. When discussing with my spouse, I usually use expressions such as ‘you always’ or ‘you never’ .
33. I can use negative statements about my spouse's personality during our discussions.
34. I can use offensive expressions during our discussions.
35. I can insult my spouse during our discussions.
36. I can be humiliating when we discussions.
37. My discussion with my spouse is not calm.
38. I hate my spouse's way of open a subject.
39. Our discussions often occur suddenly.
40. We're just starting a discussion before I know what's going on.
41. When I talk to my spouse about something, my calm suddenly breaks.
42. When I argue with my spouse, ı only go out and I don't say a word.
43. I mostly stay silent to calm the environment a little bit.
44. Sometimes I think it's good for me to leave home for a while.
45. I'd rather stay silent than discuss with my spouse.
46. Even if I'm right in the discussion, I stay silent to hurt my spouse.
47. When I discuss with my spouse, I stay silent because I am afraid of not being able to control my anger.
48. I feel right in our discussions.
49. I have nothing to do with what I've been accused of.
50. I'm not actually the one who's guilty about what I'm accused of.
51. I'm not the one who's wrong about problems at home.
52. I wouldn't hesitate to tell my spouse about her/his inadequacy.
53. When I discuss, I remind my spouse of her/his inadequacy.
54. I'm not afraid to tell my spouse about her/his incompetence.
55.   Divorce Y/N

The original data set was reviewed by the team to determine which questions would have the biggest contribution and alignment with the objective of the analysis.
21 Questions were selected to be included in the ML model analysis.
The original data frame was cleaned to include only the selected 21 Questions (columns).
    Q1.  If one of us apologizes when our discussion deteriorates, the discussion ends.
    Q6.  We don't have time at home as partners.
    Q7.  We are like two strangers who share the same environment at home rather than family.
    Q10. Most of our goals are common to my spouse.
    Q12. My spouse and I have similar values in terms of personal freedom.
    Q13  My spouse and I have similar sense of entertainment.
    Q16. We're compatible with my spouse about what love should be.
    Q18. My spouse and I have similar ideas about how marriage should be
    Q20. My spouse and I have similar values in trust.
    Q24. I can tell you what kind of stress my spouse is facing in her/his life.
    Q28. I know my spouse's hopes and wishes.
    Q29. I know my spouse very well.
    Q30. I know my spouse's friends and their social relationships.
    Q31. I feel aggressive when I argue with my spouse.
    Q32. When discussing with my spouse, I usually use expressions such as ‘you always’ or ‘you never’ .
    Q38. I hate my spouse's way of open a subject.
    Q46. Even if I'm right in the discussion, I stay silent to hurt my spouse.
    Q47  When I discuss with my spouse, I stay silent because I am afraid of not being able to control my anger.
    Q48. I feel right in our discussions.
    Q52. I wouldn't hesitate to tell my spouse about her/his inadequacy.
    Q54. I'm not afraid to tell my spouse about her/his incompetence.
    Q55. Divorce Y/N
    
By means of this analysis we hope to determine associations among the feature questions and draw possible conclusions as to which questions could play the biggest influence on whether a couple stays married or divorces.

## Description of Code:

The code will require functions, libraries, dependencies, and import of a csv file.
This code is available at Github under (https://github.com/algjor/project2_divorce_analysis).

This code was completed using the following steps.
(1) - A repository was created called project2_divorce_analysis in Git hub.
(2) - A code file was created named proj_2_divorce.ipynb on the local Git repository and pushed to GitHub on the main branch.
(3) - A development branch was created for each team member to make changes to the code.
(3) - The csv file divorce.csv was uploaded to a Resources folder within the Git hub repository.
(4) - The csv file was loaded into a Dataframe for analysis in this Machine learning model.
(5) - The data was analyzed to count the number of divorces vs. married couples and displayed.
(6) - A new data frame was then created with the features using exploratory data analysis.
(7) - A box plot was created to show the distribution of each feature against its rating.
(8) - The lowest correlation and highest correlation to divorce was then visualized using a scatter plot.
(9) - The correlation for each feature was then displayed showing the correlation of each feature to divorce.
(10) - A heat map was created to visually show the correlation between each feature along with a bar chart to show the absolute correlation.
(11) - A features and target data set were created for this analysis.
(12) - The data was then partitioned for use in testing, training, and splitting the data for this analysis.
(13) - The data was then fitted using several models: Decision Tree Model, Random Classifier Model, and Logistic Regression model.
(14) - The models accuracy was then compared to determine which model had the highest accuracy for predicting divorce.
(15) - The model accuracy was plotted using a bar chart.
(16) - The key findings of the data analysis are:
  - Random Forest Model Training Accuracy: 1.0
  - Random Forest Model Testing Accuracy: 0.9767441860465116
  - Decision Tree Model Training Accuracy: 1.0
  - Decision Tree Model Testing Accuracy: 1.0
  - Logistic Regression Model Training Accuracy: 1.0
  - Logistic Regression Model Testing Accuracy: 0.9767441860465116
