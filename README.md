Text Classification with BERT

Finetuned BERT model on a custom dataset containing tweets to classify their sentiment.
Each tweet can be classified into 8 sentiments and can have more than one categories

For e.g a tweet can be both 'joyous' and 'optimistic'

Dataset
Download link:
https://huggingface.co/datasets/sem_eval_2018_task_1

A subset of this dataset containing only English was selected. It has more than 
50,000 pairs of text and corresponding label already splitted into train and test part.
 

Training:

--BERT uncased model is used for the training
--First normal training was done on the pre-trained model for 5 epochs
--Then PEFT was done using Low Rank Adaptation(LoRA) approach which gave better 
results.


Result:
--Fine tuned model was evaluated using classification metrics Accuracy,F1,ROC-AUC curve
as the task is classification



Challenges
--Due to infrastructural challenges model could be trained for 5 epochs only which
can be increased significantly.

Example

Technologies Used:

--Langchain
--GPT 3.5
--Python
--Streamlit