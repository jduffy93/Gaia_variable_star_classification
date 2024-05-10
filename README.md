# Gaia Variable Star Classification
In this repository I will look at the data provided by the Gaia satellite (specifically Gaia D3) on variable objects, and create a classification model for variable stars.
The main aim is to learn to use image classification methods.

In the Jupyter notebook titled model.ipynb, you will find the final model.


### Metrics
---

The metrics below will only be for classification using the plotted light curves and not more complex imaging methods, like GADF (Grammian Angular Difference Frequency).

#### Light curve exmaple
![Example light curve for a cepheid variable](data/light_curve/CEP/1306279466601099904.png)

#### GADF example
![Example gadf for a cepheid variable](data/GAF/cepheid/1454784317416279168.png)

#### Binary - Cepheid vs RR Lyrae
---
The following models were made using fastai. 5000 stars from both classes were picked at random for a total of 10,000 stars. First we show models trained using a smaller model, resnet 18, and then with a larger one, resnet 34.

![Resnet18 - training](metrics/light_curve/resnet18_all_passbands_10000_remove_rejected.png)


![Resnet18 - confusion matrix](metrics/light_curve/resnet18_all_passbands_10000_remove_rejected_cm.png)

The following models were mde using fastai and resnet18. 5000 stars from both classes were picked at random for a total of 10,000 stars.

![Resnet34 - binary training](metrics/light_curve/resnet34_all_passbands_10000_remove_rejected.png)


![Resnet34 - binary confusion matrix](metrics/light_curve/resnet34_all_passbands_10000_remove_rejected_cm.png)


#### Multiclass - 24 classes
---
Here we use 5000 images for each class, where possible, however 10 of the classes do not have enough data, so we just use the maximum amount per star (curently this model is still training, and so I will only eb able to display the metrics for the mvp, which had 200 images per class.)

![Resnet18 - all clases training](metrics/light_curve/All_var_type/200_resnet18.png)

The confusion matrix is currently unreadeable due to clutter, so that still needs to be dealt with.