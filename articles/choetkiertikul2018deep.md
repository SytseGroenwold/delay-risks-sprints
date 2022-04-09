# A deep learning model for estimating story points
Source: https://github.com/jai2shukla/JIRA-Estimation-Prediction/blob/master/storypoint/IEEE%20TSE2018/preprint.pdf
Google Scholar: https://scholar.googleusercontent.com/scholar.bib?q=info:v8ARrXSPSLYJ:scholar.google.com/&output=citation&scisdr=CgXU7pQTELHQ9aZzDEE:AAGBfm0AAAAAYiB1FEEQRYIhevR1fseSOWRumxwf4oYv&scisig=AAGBfm0AAAAAYiB1FKKzHxsFO7YNS-eaKsVYHD1fG9jR&scisf=4&ct=citation&cd=-1&hl=en&scioq=Predicting+Delivery+Capability+in+Iterative+Software+Development

## Analysis
* historically, expert-based methods were mostly used
* later, model-based methods become more prevalant, to remove the subjective nature of this.
* most of the work also focuses on an entire project.
* 23313 user stories with ground truth story points
* 16 large open source projects in 9 repositories
* prediction model is to be used in conjunction, not as an alternative
* deep learning architectures: Long short term memory (LSTM) and recurrent high network (RHN)
* features are automatically learned
* Bag of Words has the issue of not knowing the semantic relation between words, and ignore word sequences. This model addresses both those issues.
* I have to research whether LSTM is used already in Dries' project. It could already be default in every single NLP package.

## Research gap
* While LSTM appears to be invaluable, it could be worthwhile to combine it with BoW to get both single-word and full-text context value from a user story's description.
* The study is 5 years old already, so it could simply be worthwhile to incorporate parts of this method with the newer updates packages to try and get an improved result.
* User story prediction is not the same as risk prediction. Applying this user story prediction difference from the actual value as a feature in other models might be a good indicator
* This paper also acknowledges that a lack of features that descibe a team working on the stories can hinder performance of this type of problem
* Therefore, it can be safe to deduce to zooming out with these specialized methods and incorporate them into a way to deduce risk per iteration is a good approach for the project