# Description of the project (below info about the files)

The ratio between the number of participants and the number of questions in psychometric questionnaires can be high. This usually makes data unsuitable for Machine Learning applications. In this notebook, I explore solutions to this problem by studying different feature selection techniques over the PID-5 dataset.

PID-5, an acronym for Personality Inventory for DSM-5, is a self-report questionnaire designed to assess personality traits according to the DSM-5 classification system. The PID-5 comprises 220 items that assess the "Big Five" personality traits: negative affectivity, detachment, antagonism, disinhibition, and psychoticism. The values are expressed in a Likert scale, which can range from 0 ("every time or frequently false") to 3 ("every time or frequently true").

The dataset's rows are 824, as the 412 participants were asked to answer the questionnaire twice: the first by answering honestly, while the second by pretending to have a mental disorder. Thus, the objective of Machine Learning models is to assess whether a participant answers honestly. I will test the following architectures: K-NN, Random Forest, Logistic Regression, Support Vector Machine, and Feed Forward Neural Network.

As I mentioned, the analysis aims to understand if applying feature selection techniques allows the models to retain good performance. I will test both model-dependent and model-agnostic methods.

After an Exploratory Data Analysis, I will create two additional datasets by applying the Principal Component Analysis. One will be obtained by transforming the original dataset using the 20% most important features; the other using the most critical variables determined by the elbow method.

Then, the aforementioned models will be fine-tuned and tested on the datasets. The main findings will be reported in the conclusions.

# Info about the files in the repository

- MD-notebook: the Jupyter Notebook with the Python code for the project;
- MD-presentation: a PowerPoint presentation of the project in .pdf format;
- MD-PID5: the dataset used for the project.
