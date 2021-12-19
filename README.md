# Convolutional-Cat-Classifier
A convolutional network that classifies two cats: Ronnie and Chuchi. It has been programmed in python via Google Collabs.
Chuchi (evil) is the white cat with brown spots and Ronnie (Good) is a ginger cat.
 
![alt text](https://github.com/bipbopbup/Convolutional-Cat-Classifier/blob/38db21306f994b11598975affd5bb19f4b625cbe/Gatingos/Chuchis/photo_2020-09-04_14-52-26.jpg)

# Input
This model has been trained with 2 image datasets which where uploaded to drive. It has been labeled with zeros (Ronnies) and 1 (Chuchis). The dataset is very small so I hope I can improve it over time.
- Chuchis: Chuchi pictures
- Ronnie: Ronnie pictures
- Pruebas: Chuchis, Ronnies and random cats to see how it classifies with new fresh data

# Output
I've implemented TensorFlow in order to assess the improvements of the model throughout my work.

So far results are pretty accurate with 60 epochs and this architecture:
Model: "sequential"

 Layer (type)                Output Shape              Param  

 conv2d (Conv2D)             (None, 498, 498, 32)      896       
                                                                 
 max_pooling2d (MaxPooling2D  (None, 249, 249, 32)     0         
 )                                                               
                                                                 
 conv2d_1 (Conv2D)           (None, 247, 247, 32)      9248      
                                                                 
 max_pooling2d_1 (MaxPooling  (None, 123, 123, 32)     0         
 2D)                                                             
                                                                 
 conv2d_2 (Conv2D)           (None, 121, 121, 64)      18496     
                                                                 
 max_pooling2d_2 (MaxPooling  (None, 60, 60, 64)       0         
 2D)                                                             
                                                                 
 conv2d_3 (Conv2D)           (None, 58, 58, 64)        36928     
                                                                 
 max_pooling2d_3 (MaxPooling  (None, 29, 29, 64)       0         
 2D)                                                             
                                                                 
 conv2d_4 (Conv2D)           (None, 27, 27, 128)       73856     
                                                                 
 max_pooling2d_4 (MaxPooling  (None, 13, 13, 128)      0         
 2D)                                                             
                                                                 
 conv2d_5 (Conv2D)           (None, 11, 11, 256)       295168    
                                                                 
 max_pooling2d_5 (MaxPooling  (None, 5, 5, 256)        0         
 2D)                                                             
                                                                 
 dropout (Dropout)           (None, 5, 5, 256)         0         
                                                                 
 flatten (Flatten)           (None, 6400)              0         
                                                                 
 dense (Dense)               (None, 250)               1600250   
                                                                 
 dense_1 (Dense)             (None, 1)                 251       
                                                                 
=================================================================
