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