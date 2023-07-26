# Healthcare-App-Experimentation

When working in realm of behavioral science as a researcher, I had the extraordinary opportunity to join forces with a dynamic start-up, determined to unlock the full potential of their app for clinical usage. Together, we were driven by the shared vision of facilitating personal health goals, and nurturing vibrant social engagement by builing a user friendly app. In this post, I will delve into one particular challenge we tackled head-on: optimizing the social event sign-up page with A/B test experiments.

## Problem Statement
Given that the app users are primarily socially avoidant individuals, we recognize the importance of maximizing their participation rates. By incorporating different message types, we aim to influence their emotional state positively and create a more engaging and encouraging sign-up process. To achieve this goal, we decided to use experimentation to find out the optimal lay-out of the page by carefully crafting the messaging and event types presented on the sign-up page.

## Experimental Design
The control group will serve as a baseline against which the effects of the two treatment groups can be compared. Treatment 1 focuses on promoting positive emotions, while Treatment 2 emphasizes the avoidance of negative emotions. These strategies are intended to make the sign-up experience more appealing and increase participation rates among socially avoidant individuals.

![image](https://github.com/yyklee/social-event-experimentation/assets/102795406/bb1a9f45-c085-4c1c-828e-c37a98bb49f3)
This is an example image that differs from the actual app used in the experiment.

* **No Message:** The control group will not receive any specific message related to emotions. They will proceed with the standard sign-up experience.
* **Positive Emotions:** Participants in this treatment group will receive messages that are specifically designed to evoke positive emotions. These messages may include uplifting and encouraging statements, images, or content.
* **Avoiding Negative Emotions:** Participants in this treatment group will receive messages that aim to avoid triggering negative emotions. The messages may provide reassurance, address potential concerns, or focus on the benefits and positive aspects of the sign-up experience.

**Randomization Unit:** The randomization unit for our experiment comprises all users who actively participated in the first round of the study. This means that all participants from the initial study will be included in the randomization process for the subsequent treatments.

**Length of Experimentation:** Although the experiment is relatively short in duration, it is important to note that we do not have control over external factors such as season and weather. These factors may introduce additional variability into the results. Despite this limitation, we believe that the one-week timeframe provides valuable insights into the effects of the treatments under investigation. The final sum of sign-up rate was used in this analysis

## Hypothesis Testing
**H0:** There is no difference in sign-up rate between the control and treatment groups. \
**H1:** There is a difference in sign-up rate between the control and treatment groups.

### 1. Assumption Check for Normality & Homogeneity
To assess the normality and homogeneity assumptions, Shapiro Test for Normality and Levene Test for homogeneity of variances were conducted on the   data sampled from the original dataset.
    
### 2. Main Analysis
As there was a violation of the normality assumption, the **Mann-Whitney U test** was used to analyze the effects of messages on the sign-up rates   for social events. Additionally, post hoc tests were performed to compare specific group differences. Mann Whitney U with Bonferroni correction      was applied to compare simultaneous confidence intervals for all possible pairwise differences and control for the family-wise error rate.
  
### 3. Guardrail Test
A guardrail test was conducted on the sampled data to assess whether the participants' distance to the location differed based on their condition.

## Results & Decisions
Based on the data analysis, the finding that the negative avoidance message was more effective than both the control group and the positive emotion group suggests that incorporating the negative avoidance message in the health care app's sign-up process could lead to higher sign-up rates for social events. Therefore, a potential business decision could be to implement the negative avoidance message as the default option for the sign-up page. 

## Citation
Based on my previous research on Social Experience and Emotional Message

