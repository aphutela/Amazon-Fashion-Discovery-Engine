
# Amazon Fashion Discovery Engine

This project involves extracting apparel details from the Amazon API and recommending similar products using NLP techniques with NLTK and machine learning models with Keras.

Personalized product recommendations offer an alternative way to navigate online shops, helping more people find products they need—even those they hadn't considered. By building a recommendation engine, we can suggest similar products on any e-commerce website, such as Amazon.com.
# Datasets

1. [apparel_data](https://www.kaggle.com/datasets/ajaysh/women-apparel-recommendation-engine-amazoncom#tops_fashion.json)
2. [Preprocessed Data](https://drive.google.com/file/d/1rHpQn9bAQAqWFx564Wn4ohPnOZ0Wmqf3/view?usp=sharing)
3. Trained CNN Model (VGG16)

    [16k_data_features_asins](https://drive.google.com/file/d/12CQpeZMOlp0ft1iEKYFSAd_iNISA2gdw/view?usp=sharing)

# Model Description
Given a JSON file containing 180k apparel images from Amazon.com, we need to recommend similar apparel based on the product ID and the number of recommendations desired. Each recommended item will be based on the following fields:

Although we had 19 features, we used only the most important ones.
1. asin  ( Amazon standard identification number)

2. brand ( brand to which the product belongs to )

3. color ( Color information of apparel, it can contain many colors as   a value ex: red and black stripes) 

4. product_type_name (type of the apperal, ex: SHIRT/TSHIRT)

5. medium_image_url  (url of the image)

6. title (title of the product)

7. formatted_price (price of the product)

We will utilize a total of seven approaches for recommending apparel, as follows:

1. BoW (Bag of Words)
2. Tf-Idf (Term frequency - Inverse Document frequency)
3. Idf
4. Weighted similarity (Using Title + Brand and Color)
5. CNN (VGG16)

# Conclusion
We trained the five models and recommended similar top 20 apparels with the least euclidean distance for each model.

We calculated the average euclidean distance for each model by taking the mean and compared them using the bar graph.

# Results 
We determined that the order of the best recommendation performance is as follows:

1. Tf-Idf
2. Weighted similarity (Tf-Idf)
3. BoW
4. Idf
5. CNN









