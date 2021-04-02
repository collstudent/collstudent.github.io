---
layout: post
title:  Loggers in PyTorch Lightning
category: PyTorch 
description: How to use TFLogger and CSVLogger in PyTorch Lightning
---

PyTorch Lightning has a builtin logger that can be used to log metrics and hyperparameters. Internally, it uses TensorBoard. However, it has a few caveats
* Logging is buggy; I couldn't use it to log accuracy in the `_epoch_end` method
* It doesn't support advanced functionality such as computational graphs
* There is no way to control the x-axis parameter

There are two workarounds

**(1) Use TensorBoardLogger**

This explicitly uses TensorBoard.

First you need to import it
```
from pytorch_lightning.loggers import TensorBoardLogger
```
It needs to be passed to the trainer. Then, inside the training/validation steps, you can log metrics by calling the method `self.logger.experiment.add_scalar`. Note that the parameter on the x-axis can also be specified.

**(2) Use CSVLogger**

This logs to CSV files, which can be used to plot data using matplotlib (for old-fashioned people like me!).

First you need to import it
```
from pytorch_lightning.loggers import CSVLogger
```
It needs to be passed to the trainer. Then, inside the training/validation steps, you can log metrics by calling the method `self.logger.log_metrics`

For complete working example on the MNIST dataset, [please look at the notebooks here.](https://github.com/mmg10/logger) 
