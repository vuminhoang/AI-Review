# Wandb: Tracking and Visualizing Training Progress
Wandb (Weights and Biases) is a powerful tool for tracking and visualizing machine learning experiments. 
It integrates with some popular DL frameworks like PyTorch and Keras Tensorflow...
providing an easy way to monitor the training process and share results with your team or community.

## How to use
- Visit their website at https://wandb.ai/site/
- Log in or sign up.
- In your notebook or python file:
```
import wandb
wandb.login()
```
- Click in the link that they provides, you will automatically receive the login token. Use it to continue!
- Define log metric:
```
wandb.log({"loss": loss, "accuracy": accuracy})
```
Or you can enter any metrics that you want to track!

- Define init:
```
wandb.init(
      # your project on website name
      project="lstm_sentiment_analysis",
      # name of this version
      name=f"ori_1lstm_new_", 
      # Track hyperparameters and run metadata
      config={
      "learning_rate": lr,
      "architecture": "LSTM",
      "dataset": "vsa",
      "epochs": num_epochs,
      })

```
