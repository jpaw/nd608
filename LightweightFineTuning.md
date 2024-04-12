## Results of lightweight finetuning

Used distilbert, because BERT type models should be good for sequence classification.
Used rotten tomatoes data set, for good size and already existing split into training, validation and test. Due to size, only use 33% of that.
Used LoRA finetuning.
Switched "accuracy" metric now to "f1".

Evaluation of model out of the box: f1 = 0.66, loss 0.70

Trained LoRA for 4 epochs, using q_lin, v_lin (< 1% if parameters trained compared to full training).
Training time on RTX 3090: 2 minutes 22 seconds.

Evaluation of model after epoch 4: f1 = 0.81, loss 0.20  (improvement on f1, much smaller loss)

Real test after reloading: f1 = 0.81 (as before), test loss 0.43 (higher than after training)


(full history on github: https://github.com/jpaw/nd608)
