# G2PTrainer
A hard fork of the G2P training code from [OpenUTAU’s repository](https://github.com/stakira/OpenUtau/tree/master/py), extended with modifications to enable more flexible experimentation with training parameters.  

## What’s New?  
- **Integrated `pytorch-optimizer`**: This adds access to a wider variety of optimizers and learning rate schedulers, making it easier to experiment with training stability, performance improvements, or avoiding NaN issues.  

## How to Use  
- Edit your `.yaml` configuration file (or the default settings inside the input dictionary in the Colab notebook) to define parameters for optimizers and learning rate schedulers.  
- For optimizers, you can use either:  
  - `pytorch_optimizer.<OptimizerName>`  
  - `torch.optim.<OptimizerName>`  
- For learning rate schedulers, you can also use either:  
  - `torch.optim.lr_scheduler.<SchedulerName>`  
  - `pytorch_optimizer.<SchedulerName>`
 
- For more information, check the original repo.

Both optimizers and schedulers support full parameter customization through the `.yaml` file (or inside the Colab cell).

> **Credits**: Based on the original OpenUTAU repository.  


