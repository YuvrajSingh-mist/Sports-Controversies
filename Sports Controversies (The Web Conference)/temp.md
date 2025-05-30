 \item \textit{Probing Analysis of LLM outputs}

     

     We ran probing analysis on the attention outputs of the fine-tuned (denoted as positive class) and non-fine-tuned (negative class) versions of the LLama 3.1-8 b-Instruct model, denoted by Fig 2 and 3, respectively.

     The attention outputs is particularly high for the tokens - \texttt{exact\_answer\_first} and \texttt{exact\_answer\_last} for fine tuned model for majority of the layers, while for the non fine tuned one, it was high for all the tokens and layers, not consolidating to tokens particular to the answer to be generated, or the labels.
     
     These heatmaps were generated by resp. F1 scores of a logistic classifier's accuracy were 82% and 23% resp. for both the model.
     Due to the high metric (f1) for the fine-tuned model, we termed the labels generated to be a 'positive class' and for the other model to be a 'negative class' (low f1 score).
     
     We can see that the heatmap for the positive class model has high attention outputs for the tokens corresponding to the labels to be generated or the answer in particular, while it attends to every token or haywire for the non-fine-tuned negative class model.



          The attention outputs is particularly high for the tokens - \texttt{exact\_answer\_first} and \texttt{exact\_answer\_last} for fine tuned model for majority of the layers, while for the non fine tuned one, it was high for all the tokens and layers, not consolidating to tokens particular to the answer to be generated, or the labels.
     
     These heatmaps were generated by resp. the F1 scores for a trained logistic classifier whose accuracy were 82\% and 23\% resp. for both the fine-tuned models.
     Due to the high metric (F1) for the fine-tuned model, we termed the labels generated to be a 'positive class' and for the non-fine-tuned model to be a 'negative class' (low F1 score).
     
     We can see that the heatmap for the positive class or the fine-tuned model has high attention outputs for the tokens corresponding to the labels to be generated or the answer in particular, while it attends to every token or haywire for the non-fine-tuned or negative class model.
    