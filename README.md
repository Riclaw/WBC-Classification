# WBC-Classification

## Task:
The task we have addressed with this project was to correctly classify 8 different types of white blood cells : Eosinophils, Erythroblasts, Immature Granulocytes, Lymphocytes, Neutrophils, Monocytes, and
Platelets using the CNN. This project was part of the 'Deep Learning for Computer Vision' 20600.

## Short explanation of our approach

To solve this task, 15092 images of different blood cells with dimension 48x48 have been provided. 
Regarding the preprocessing and given that the target is always centred in the image, we decided to
apply translation, rotation and flip assuming the usage of the model in a real-world context, where
the images may have different properties, i.e. the cell is not on the corners of the image. Later on, we decided to do data augmentation, by concatenating sets of randomly rotated, flipped and translated images. The last NN we created for this task was a CNN made of 18 convolutional layers, batch normalization, skip connections and AdamW optimizer. 

[Here you can find the full report](link)

## General requirements

```
tensorflow==2.14.0
scipy==1.11.3
matplotlib==3.7.1
numpy==1.23.5
scikit_learn==1.2.2
cv2==4.8.0
```
## Results

These are the scores for the different models implemented in the notebook:

![image](https://github.com/Riclaw/WBC-Classification/assets/27282059/f1d616bc-b090-4b47-a81d-0add0d3b640d)

Class activation map (CAM) example:

![image](https://github.com/Riclaw/WBC-Classification/assets/27282059/8b81a8ff-503e-407a-8da8-38d48013f124)

## Credits

| Author             | Contact                       
| ----------------   | ------------------------------
| Riccardo Valdo     | riccardo.valdo@studbocconi.it         
| Lorenzo d'Imporzano | lorenzo.dimporzano@studbocconi.it 
| Edoardo Morresi | edoardo.morresi@studbocconi.it 


