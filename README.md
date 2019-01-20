# twitter-bot
A bot for Twitter. You can follow users in a specific location or tweeting specific words and unfollow those who dont follow-you-back (and are not included in  whitelist.txt)


## Usage

Follow people who tweeted a word (**query**), limited to the **limit** value:
```
python twitter-bot.py -q {query} -l {limit} -o follow**
```

Follow people who tweeted in a location (**geocode**), limited to the **limit** value:
```
python twitter-bot.py -g {geocode} -l {limit} -o follow**
```

Unfollow people who do not follow you back:
```
python twitter-bot.py -o unfollow**
```


## Example

Follow 5 people who tweeted 'oscp':
```
python twitter-bot.py -q "oscp" -l 5 -o follow
```
![Screenshot](images/img1.png)

Follow 7 people tweeting in 40.432,-3.708:
```
python3 twitter-bot.py -g "40.432,-3.708,10km" -l 7 -o follow
```
![Screenshot](images/img2.png)

Unfollow people who i follow butt they do not follow me back:
```
python3 twitter-bot.py -o unfollow
```
![Screenshot](images/img3.png)


## Requirements

Python 2.x:

```
sudo pip install -r requirements.txt
```

Python 3.x:

```
sudo pip3 install -r requirements.txt
```

*Create a twitter account and a twitter app, and fill the **config.py** file*

## Note

Tested both in Python2.x (2.7.15rc1) and Python 3.x (3.6.7)

