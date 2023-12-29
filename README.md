# Text Classification with BERT

Finetuned BERT model on a custom dataset containing tweets to classify their sentiment.
Each tweet can be classified into 8 sentiments and can have more than one categories

For e.g a tweet can be both 'joyous' and 'optimistic'

## Dataset<br>
Download link:
https://huggingface.co/datasets/sem_eval_2018_task_1

A subset of this dataset containing only English was selected. It has more than 
50,000 pairs of text and corresponding label already splitted into train and test part.
 

## Training:<br>

--BERT uncased model is used for the training<br>
--First normal training was done on the pre-trained model for 5 epochs<br>
--Then PEFT was done using Low Rank Adaptation(LoRA) approach which gave better 
results.<br>


## Result:<br>
--Fine tuned model was evaluated using classification metrics Accuracy,F1,ROC-AUC curve
as the task is classification



## Challenges:<br>
--Due to infrastructural challenges model could be trained for 5 epochs only which
can be increased significantly.

