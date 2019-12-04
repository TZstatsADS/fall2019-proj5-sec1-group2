# ADS Project 5: 

Term: Fall 2019

+ Team 2
+ Projec title: "Machine Learning Fairness" Classification 
+ Team members
	+ Chongyu He (ch3379)
+ Project summary: Given some information about a person, your task is to predict if the person's annual income level is greater than 50K$ or not. 
+ Notations: A=gender, Ŷ=prediction on the income level, Y=ground-truth income level
+ Final Score: Accuracy:= ℙ[Ŷ =Y]   
	       DDP:= |ℙ[Ŷ =1|A=0]−ℙ[Ŷ =1|A=1]|   
	       Th:= 0.1   
	       If DDP>Th,Bias:= 7^(DDP−Th)−1, else, Bias:= 0   
	       Score:= Accuracy−Bias   
	
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
