# Ishan's News Classifier API

An API developed by using the FastAPI library and uses an NLP model to classify the category of the news in the Swahili language.

API URL: [https://limitless-forest-00896.herokuapp.com/news-prediction/](https://limitless-forest-00896.herokuapp.com/news-prediction/)

## News Categories

The NLP model will classify news by using the following categories.

1. National
2. Sports
3. Economy
4. International
5. Entertainment


## Example 
How to use the API URL in your own application.The example below uses python programming language.

```python
import requests as r

# sample news article
news = "Chelsea midfielder Romelu Lukaku has been linked with a move to former club Inter Milan but the 28-year-old Belgian is set to move to Stamford Bridge. (Mirror)"

# make prediction
keys = {"news": news}
prediction = r.get(
    "https://limitless-forest-00896.herokuapp.com/news-prediction/", params=keys
)

# collect and print the result
results = prediction.json()
print(results["prediction"])
print(results["Probability"])
````

**Note:** You can use the API URL in any programming language, you just need to follow the instruction of a particular langauge to access and use this API.


## Issues 

Incase you have any difficulties or issues while trying to run the script
you can raise it on the issues section. 

## Pull Requests

If you have something to add or new idea to implement, you are welcome to create a pull requests on improvement.

## Give it a Star

If you find this repo useful , give it a star so as many people can get to know it.

## Credits

All the credits to [Davis David ](https://twitter.com/Davis_McDavid)
