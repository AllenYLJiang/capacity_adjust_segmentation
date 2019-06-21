# capacity_adjust_segmentation

1. 100 times speed up
train_trainval_21_22_31_components.prototxt and vgg_100_times_speed_up.caffemodel denote the model for human parsing with 100 times speed up.

2. evaluation of mutual information between hidden activations and input images:
Here we provide an example on evaluating the mutual information. 
We've pre-trained a segmentation model with decoders mapping the output of each layer to its input:

https://drive.google.com/file/d/1OeHmBgETwi3ro1by2n6YwxdXStETuJCG/view?usp=sharing

https://drive.google.com/file/d/1kLQjsHoQOfzO_jroSA1SZvLEJeyw3He-/view?usp=sharing

For instance, we've obtained the activations on the 1st layer, 2nd layer and 3rd layer through forward propogation. Then we try to recover the input using the three sets of activations. 
The first set can best recover the inputs while the third set performs the worst. 
