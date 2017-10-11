## Building CNN image classification models using keras(Backend tensorflow)
It uses data that can be downloaded at:
http://www.ee.surrey.ac.uk/CVSSP/demos/chars74k/
It can work with multiple classes, for this implimentation we are working on identifying numbers
In our setup, we:
- created a data/ folder
- created train/ and validation/ subfolders inside data/
- created 0/, 1/, 2/, 3/, 4/, 5/, 6/, 7/, 8/ and 9/ subfolders inside train/ and validation/
- put the cat pictures index 0-800 in data/train/...
- put the cat pictures index 8001-1000 in data/validation/...
So that we have 800 training examples for each class, and 200 validation examples for each class.
In summary, this is our directory structure:
```
data/
    train/
        0/
            img0_001.jpg
            img0_002.jpg
            ...
        1/
            img1_001.jpg
            img1_002.jpg
            ...
		2/
            img2_001.jpg
            img2_002.jpg
            ...
    validation/
        0/
            img0_801.jpg
            img0_802.jpg
            ...
        1/
            img1_801.jpg
            img1_802.jpg
            ...
		2/
            img2_801.jpg
            img2_802.jpg
            ...


Available Customizations:
line 16: Update image size
line 46: dropout rate
line 47: number of output classes

#Output 
runfile('.../CNN-image-classifier-categorical-/demo.py', wdir='.../CNN-image-classifier-categorical-')
Found 8000 images belonging to 10 classes.
Found 2160 images belonging to 10 classes.
Epoch 1/15
125/125 [==============================] - 111s - loss: 1.7287 - acc: 0.4405 - 
val_loss: 0.9860 - val_acc: 0.7262
Epoch 2/15
125/125 [==============================] - 119s - loss: 1.0214 - acc: 0.7035 - 
val_loss: 0.6904 - val_acc: 0.8113
Epoch 3/15
125/125 [==============================] - 119s - loss: 0.7495 - acc: 0.7735 - 
val_loss: 0.4695 - val_acc: 0.8775
Epoch 4/15
125/125 [==============================] - 108s - loss: 0.6005 - acc: 0.8140 - 
val_loss: 0.3593 - val_acc: 0.9175
Epoch 5/15
125/125 [==============================] - 126s - loss: 0.4774 - acc: 0.8625 - 
val_loss: 0.3519 - val_acc: 0.9113
Epoch 6/15
125/125 [==============================] - 109s - loss: 0.3981 - acc: 0.8600 - 
val_loss: 0.2741 - val_acc: 0.9300
Epoch 7/15
125/125 [==============================] - 110s - loss: 0.3124 - acc: 0.9075 - 
val_loss: 0.1990 - val_acc: 0.9463
Epoch 8/15
125/125 [==============================] - 125s - loss: 0.2728 - acc: 0.9105 - 
val_loss: 0.1964 - val_acc: 0.9425
Epoch 9/15
125/125 [==============================] - 118s - loss: 0.2548 - acc: 0.9200 - 
val_loss: 0.2318 - val_acc: 0.9413
Epoch 10/15
125/125 [==============================] - 128s - loss: 0.2566 - acc: 0.9215 - 
val_loss: 0.2443 - val_acc: 0.9425
Epoch 11/15
125/125 [==============================] - 130s - loss: 0.2261 - acc: 0.9290 - 
val_loss: 0.1996 - val_acc: 0.9437
Epoch 12/15
125/125 [==============================] - 114s - loss: 0.2157 - acc: 0.9265 - 
val_loss: 0.2057 - val_acc: 0.9387
Epoch 13/15
125/125 [==============================] - 105s - loss: 0.2147 - acc: 0.9320 - 
val_loss: 0.1748 - val_acc: 0.9513
Epoch 14/15
125/125 [==============================] - 98s - loss: 0.2169 - acc: 0.9280 - 
val_loss: 0.2453 - val_acc: 0.9300
Epoch 15/15
125/125 [==============================] - 143s - loss: 0.1867 - acc: 0.9405 - 
val_loss: 0.1541 - val_acc: 0.9587
Accuracy achieved on validation dataset after 15 epoch = 0.9587