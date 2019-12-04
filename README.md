# ADS Project 5: 

Term: Fall 2019

+ Team 2
+ Projec title: "Machine Learning Fairness" Classification 
+ Team members
	+ Chongyu He (ch3379)
+ Project summary: Given some information about a person, your task is to predict if the person's annual income level is greater than 50K$ or not. Rather than purely maximizing prediction accuracy, I would try to maximize accuracy while achieving the fairness requirement. Specifically, my model must follow a relaxed version of demographic parity for the binary sensitive attribute "gender".
+ Notations: A=gender, Ŷ=prediction on the income level, Y=ground-truth income level
+ Final Score: 
Accuracy:= ℙ[Ŷ =Y]   
DDP:= |ℙ[Ŷ =1|A=0]−ℙ[Ŷ =1|A=1]|   
Th:= 0.1   
If DDP>Th,Bias:= 7^(DDP−Th)−1, else, Bias:= 0   
Score:= Accuracy−Bias  

+ Final Score: 
Logistic Regression: 80.0% accuracy, 0.05 DDP Value, 0.80 Score  
XGBoost: 86.5% accuracy, 0.17 DDP Value, 0.75 Score   
Random Forest: 86.7% accuracy, 0.20 DDP Value, 0.70 Score   
1 XGBoost + 1 Logistic Regression: 82.2% accuracy, 0.07 DDP Value, 0.82 Score   
2 XGBoost + 1 Logistic Regression: 83.6% accuracy, 0.095 DDP Value, 0.84 Score
	
**Contribution statement**: ([default](doc/a_note_on_contributions.md)) All team members contributed equally in all stages of this project. All team members approve our work presented in this GitHub repository including this contributions statement. 

Following [suggestions](http://nicercode.github.io/blog/2013-04-05-projects/) by [RICH FITZJOHN](http://nicercode.github.io/about/#Team) (@richfitz). This folder is orgarnized as follows.

```
proj/
├── lib/
├── data/
├── doc/
├── figs/
└── output/
```

Please see each subfolder for a README file.
