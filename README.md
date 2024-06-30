# Image-Caption-Generator

# About

1. The goal of this project is to create a system that generates descriptive text for a given image, essentially producing a 'caption' for the image.
2. Utilized the Flickr8k dataset, which includes 8,091 images, each accompanied by 5 captions.
3. Employed an Encoder-Decoder model architecture, using a Pre-Trained VGG16 network as the Encoder and an LSTM cell with Bahdanau Attention as the Decoder.
4. Achieved a corpus BLEU-1 score of 0.539 and BLEU-2 score of 0.313 on the test dataset(flickr8k) for caption generation accuracy.

# Model Preview
![Model](/ModelPreview.jpg)

# Dataset
You can access the test dataset i.e., flickr8k: [here](https://www.kaggle.com/datasets/adityajn105/flickr8k).

# Steps to run this on your local computer:

- Clone this repository
```
https://github.com/Arin13-03/Image-Caption-Generator.git
```

- Download the requirements of the environment using 
```
pip install -r requirements.txt
```
- Download the model and place it into the same root directory as app.py. You can download the model [here](https://drive.google.com/file/d/1xg9cRHrjhZugeL8A3XKdE15ob0AUUdFL/view?usp=sharing).
- Run app.py file to open the website
```
streamlit run app.py
```

# Website Screenshots
- This is the homepage you will see in the browser. To upload your image, click on browse and select an image from your computer.
![Homepage](/App_Preview.png)
- The results will appear below your image under the 'Generated Caption' heading
![Output](/Result.png)
