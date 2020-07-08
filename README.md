# ElonJsonTokenism
Tokenising data scrapped about Elon Musk from twitter.

Issues and Errors. 

I'm running into many decoding issues but I assume its from the JSON file not being correctly formatted but I don't know how to validate what is wrong and where it's wrong without using online JSON Validators which are telling me the format is valid.

I'm not sure where the issues is and have been searching through StackOverflow, been asking on StackOverflow but can't find an answer. I was told the JSON file wasn't formatted properly with incorrect ',' and '{' but have validated the file without any issues. 

Traceback (most recent call last):
  File "ElonSorter.py", line 45, in <module>
    tweet = json.loads(line.decode('utf-8'))
AttributeError: 'str' object has no attribute 'decode'
  
According to stackoverflow the issue is to do with empty lines produced by the Twitter scraper. 
Using the answer here at "https://stackoverflow.com/questions/44785611/pre-process-tweets-in-a-json-file" I tried using the method in the answer to no success, but the original poster updated their question and stated the tokeniser doesn't seem to work for a whole file of tweets but only for one or two at a time. As I have over 9000 tweets, I did not know what to do next. 
