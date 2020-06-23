# Style generator [Video/Image]
The application segment person from the image and mask person or background with the reference style image.

### Summary:
Stylized image is generated using a reference image. The segementation model seperates humans from the background. Then the style is applied to either background or the person as per choice.

### Result:

<table>
    <tr align="center">
    <td align="center"><b>Input Image ----></b> </td>
    <td align="center"><img src="/Outputs/3.png" height=350 width=290></td>
    <td></td>
  </tr>
  <tr>
    <td align="center"><b>1) Style applied to background</b></td>
     <td align="center"><b>2) Style applied to persons</b> </td>
     <td align="center"><b>3) Style normalized to person</b></td>
  </tr>
  <tr>
    <td align="center"><img src="/Outputs/3_style1_1.png" height=350 width=290></td>
    <td align="center"><img src="/Outputs/3_style1_2.png" height=350 width=290></td>
    <td align="center"><img src="/Outputs/3_style1_3.png" height=350 width=290></td>
    </tr>
 </table>

 
### Requirements:
1. Opencv
2. Numpy
3. Tensorflow 2.x for style transfer model
4. Tensorflow 1.x for segmentation model
5. JSON
6. Flask
7. flask_ngrok
8. Requests

### Pre-Trained models used:
1. Style transfer model
https://tfhub.dev/google/magenta/arbitrary-image-stylization-v1-256/2 

2. deeplab version 3
http://download.tensorflow.org/models/deeplabv3_pascal_train_aug_2018_01_04.tar.gz

#### Citation:
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
