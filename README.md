# Style generator [Video/Image]
Using style transfer and Deep learning to Stylize a person or background

### Summary:
Image/video is supplied to the model it extracts out all persons and then apply a style to the image. The style can be anything in the form of image. The machine will learn the style and will apply to original image.

### Outputs:
Output is in the form of JSON file containing 3 images
1. Stlye applied only to background
2. Style applied to persons alone
3. Style applied to person normalized with background

### Requirements:
1. Opencv
2. Numpy
3. Tensorflow 2.x for style transfer model
4. Tensorflow 1.x for segmentation model
5. JSON
6. Flask
7. flask_ngrok
8. Requests

### Pre-Trained model used:
1. Style transfer model
https://tfhub.dev/google/magenta/arbitrary-image-stylization-v1-256/2 

2. deeplab version 3
http://download.tensorflow.org/models/deeplabv3_pascal_train_aug_2018_01_04.tar.gz

##### Citation:
@inproceedings{deeplabv3plus2018,
  title={Encoder-Decoder with Atrous Separable Convolution for Semantic Image Segmentation},
  author={Liang-Chieh Chen and Yukun Zhu and George Papandreou and Florian Schroff and Hartwig Adam},
  booktitle={ECCV},
  year={2018}
}

### References:

1. Style transfer model from tensorflow hub
https://tfhub.dev/google/magenta/arbitrary-image-stylization-v1-256/2

2. Deep lab model from Tensorflow Research
https://github.com/tensorflow/models/tree/master/research/deeplab 
