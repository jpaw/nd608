## Results of lightweight finetuning

Used distilbert, because BERT type models should be good for sequence classification.
Used rotten tomatoes data set, for good size and already existing split into training, validation and test.
Used LoRA finetuning.

- evaluation of model out of the box: accuracy 0.494, loss 0.694 (initial commit)
- evaluation of model after training classifier: accuracy 0.820, loss 0.425 (quite good, shows that BERT was a good choice)

Trained LoRA for 4 epochs, using q_lin, v_lin and classifier (< 1% if parameters trained compared to full training).
Training time on RTX 3090: 9 minutes 17 seconds.

- evaluation of model after epoch 4: accuracy 0.834, loss 0.233  (slight improvement on accuracy, significantly smaller loss reported)

Real test: accuracy 0.824, loss 0.430 (better than before LoRA, but a bit worse than the training reported, probably within margin of error>)
