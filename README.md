
## Problem Statement

An education company named X Education sells online courses to industry professionals. On any given day, many professionals who are interested in the courses land on their website and browse for courses. 

The company markets its courses on several websites and search engines like Google. Once these people land on the website, they might browse the courses or fill up a form for the course or watch some videos. When these people fill up a form providing their email address or phone number, they are classified to be a lead. Moreover, the company also gets leads through past referrals. Once these leads are acquired, employees from the sales team start making calls, writing emails, etc. Through this process, some of the leads get converted while most do not. The typical lead conversion rate at X education is around 30%.

Now, although X Education gets a lot of leads, its lead conversion rate is very poor. For example,if, say, they acquire 100 leads in a day, only about 30 of them are converted. To make this process more efficient, the company wishes to identify the most potential leads, also known as ‘Hot Leads’. If they successfully identify this set of leads, the lead conversion rate should go up as the sales team will now be focusing more on communicating with the potential leads rather than making calls to everyone. A typical lead conversion process can be represented using the following funnel:

![Lead Conversion Process - Demonstrated as a funnel](https://cdn.upgrad.com/UpGrad/temp/189f213d-fade-4fe4-b506-865f1840a25a/XNote_201901081613670.jpg)

**Lead Conversion Process - Demonstrated as a funnel**

As you can see, there are a lot of leads generated in the initial stage (top) but only a few of them come out as paying customers from the bottom. In the middle stage, you need to nurture the potential leads well (i.e. educating the leads about the product, constantly communicating etc. ) in order to get a higher lead conversion.

X Education has appointed you to help them select the most promising leads, i.e. the leads that are most likely to convert into paying customers. The company requires you to build a model wherein you need to assign a lead score to each of the leads such that the customers with a higher lead score have a higher conversion chance and the customers with a lower lead score have a lower conversion chance. The CEO, in particular, has given a ballpark of the target lead conversion rate to be around 80%.

## Solution Approach

- Get data source for analysis and understand the data
- Clean and prepare the data
- Exploratory Data Analysis
- Model Building
	- Feature Scaling
	- Splitting the data into Test and Train dataset.
	- Building a logistic Regression model and calculate Lead Score. 
- Model Evaluation
	- Evaluating the model by using different metrics 
		- Accuracy
		- Specificity and Sensitivity 
		- Precision and Recall. 
- Applying the best model in Test data based on the Sensitivity and Specificity Metrics.
- Making prediction on the test data set

## Conclusion


- While we have checked both Sensitivity-Specificity as well as Precision and Recall Metrics, we have considered the optimal cut off based on Sensitivity and Specificity for calculating the final prediction. 
- Accuracy, Sensitivity and Specificity values of test set are around `80.3 %` ,  `79.4 %` and `80.8 %` which are approximately closer to the respective values calculated using trained set. 
- Also the lead score calculated shows the conversion rate on the final predicted model is around `80 %`
- The top 3 variables that contribute for lead getting converted in the model are 
    - Lead Origin Lead Add Form
    - Last Activity_Others
    - Last Notable Activity_Unreachable
- Hence overall this model seems to be acceptable.

## Reference Files 

- [Notebook](./Lead_Score_Notebook.ipynb)
- [Summary](./Lead_Score_Summary.pdf)
- [Presentation](./Lead_Score_Case_Study_Presentation.pdf)
- [Subjective Answers](./Lead_Score_Subjective_Answers.pdf)