# Healthcare-App-Experimentation

When working in realm of behavioral science as a researcher, I had the extraordinary opportunity to join forces with a dynamic start-up, determined to unlock the full potential of their app for clinical usage. Together, we were driven by the shared vision of facilitating personal health goals, and nurturing vibrant social engagement by builing a user friendly app. In this post, I will delve into one particular challenge we tackled head-on: optimizing the social event sign-up page with A/B test experiments.

## Problem Statement
Given that the app users are primarily socially avoidant individuals, we recognize the importance of maximizing their participation rates. By incorporating different message types, we aim to influence their emotional state positively and create a more engaging and encouraging sign-up process. To achieve this goal, we decided to use experimentation to find out the optimal lay-out of the page by carefully crafting the messaging and event types presented on the sign-up page.

## Experimental Design
The control group will serve as a baseline against which the effects of the two treatment groups can be compared. Treatment 1 focuses on promoting positive emotions, while Treatment 2 emphasizes the avoidance of negative emotions. These strategies are intended to make the sign-up experience more appealing and increase participation rates among socially avoidant individuals.

![image](https://github.com/yyklee/social-event-experimentation/assets/102795406/a7d2ebc1-a14e-4440-9214-8b82e1d361f2)
Prototype Image: Control (A) vs Treatment (B) vs Treatment (C)

* **No Message:** The control group will not receive any specific message related to emotions. They will proceed with the standard sign-up experience.
* **Positive Emotions:** Participants in this treatment group will receive messages that are specifically designed to evoke positive emotions. These messages may include uplifting and encouraging statements, images, or content.
* **Avoiding Negative Emotions:** Participants in this treatment group will receive messages that aim to avoid triggering negative emotions. The messages may provide reassurance, address potential concerns, or focus on the benefits and positive aspects of the sign-up experience.

**Randomization Unit:** The randomization unit for our experiment comprises all users who actively participated in the first round of the study. This means that all participants from the initial study will be included in the randomization process for the subsequent treatments.
**Length of Experimentation:** Although the experiment is relatively short in duration, it is important to note that we do not have control over external factors such as season and weather. These factors may introduce additional variability into the results. Despite this limitation, we believe that the one-week timeframe provides valuable insights into the effects of the treatments under investigation. The final sum of sign-up rate was used in this analysis

## Hypothesis Testing
H0: No difference in sign-up rate btw control & treatment group \
H1: Difference in sign-up rate btw control & treatment group

### 1. Assumption Check for Normality & Homogeneity
  - Shapiro Test for Normality
  - Levene Test for homogeneity of variances
    
### 2. Hypothesis Testing
  - After conducting a **Two-Way ANOVA** to analyze the effects of two factors (group A vs. B) and (group A vs. C) on the sign-up rates for social events, you can perform post hoc tests to compare specific group differences.
  - **Honestly Significant Difference (Tukey's HSD) test** was used to compare simultaneous confidence intervals for all possible pairwise differences and control for family-wise error rate.
  
### 3. Guardrail Test
  - Check whether or not their distance to the location differs by condition. 

## Decisions
Based on the information provided, it seems that the negative avoidance message tested in the study was found to be more effective than the control group or the positive emotion group. This suggests that the negative avoidance message had a positive impact on the sign-up rate. However, due to the lack of users in this experiment, we had to use the whole cohort of participants in this test and results to be applied to the next cohort of users.

## Citation
Based on my previous research on Social Experience and Emotional Message (Exp1_syntax.R ~ Exp3_syntax.R) 
