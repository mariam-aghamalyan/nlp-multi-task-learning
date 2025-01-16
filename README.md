# Multi-Task Learning with NLP
***Detecting Emotions, Violence, Hate from text***
### This model is designed to perform three tasks at the same time:

* Emotion Detection: Identifying emotions in text (e.g., happy, sad, angry, fear).
* Violence Detection: Classifying text into types of violence like physical, emotional, or sexual.
* Hate Speech Detection: Detecting offensive or hateful language.

### The model is built on a shared-core architecture:

* Input Layers: Each task has its own input layer to process task-specific data.
* Shared Core Layers: These include embeddings, LSTMs, pooling, and dropout layers that are shared across tasks.
* Output Layers: Separate output layers handle predictions for each task.

### The Datasets
I used publicly available datasets tailored for each task:

* [Emotion Detection](https://www.kaggle.com/datasets/nelgiriyewithana/emotions): Labeled data with various emotional categories.
* [Violence Detection](https://www.kaggle.com/datasets/gauravduttakiit/gender-based-violence-tweet-classification?select=Train.csv): Text labeled with types of violence.
* [Hate Speech Detection](https://www.kaggle.com/datasets/mrmorj/hate-speech-and-offensive-language-dataset): Annotations marking text as offensive or hateful.

### Dataset Labels
The datasets used in this project are annotated with specific labels for each task. Below is a breakdown of the labels and their meanings:

#### Emotion Detection

* 0: Sadness
* 1: Joy
* 2: Love
* 3: Anger
* 4: Fear
* 5: Surprise
 
#### Violence Detection

* 0: Harmful Traditional Practice
* 1: Physical Violence
* 2: Economic Violence
* 3: Emotional Violence
* 4: Sexual Violence
 
#### Hate Speech Detection

* 0: Hate Speech
* 1: Offensive Speech
* 2: Neither

