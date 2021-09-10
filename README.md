# Product-Category-Prediction
Machine learning pipeline to predict relevant categories based on a product name and product description, using NLP and Deep learning concepts.
We are explected to build an api that can predict possible categories for any product. We will be using product name and it's description to find relevant categories.

## Machine learning pipeline
![alt text](https://github.com/prakhargurawa/Product-Category-Prediction/blob/main/download.png?raw=true)

The dataset can be found here: https://github.com/BestBuyAPIs/open-data-set

It contains data in the form of three json files : categories.json, products.json and stores.json

The stores.json contains information like store id, type, name, address, hours etc which is not relevant for this task at this point. The categories.json list different categories from which our predictions will belong to, but will not be used for our work. The file used is product.json which contains the product names, description and their categories, from which our model will learn to tag categories to new products.

As each instanse can belong to multiple categories, so these types of problems are known as multi-label classification problem, where we have a set of target labels. If there are multiple categories but each instance is assigned only one, therefore such problems are known as multi-class classification problem.

Multi-class problem acknowledge that all the classes are mutually exclusive, but in our case it is not as a product can belong to multiple classes/categories.
