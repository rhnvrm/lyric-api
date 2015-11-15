# lyric-api
API that returns lyrics after searching on lyrics.wikia.com based on Artist and Song.

##Deploy on Heroku

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

##Deployed at: 
https://lyric-api.herokuapp.com/api/ <del>and
http://128.199.199.233:8081/api/</del>

Usage: https://lyric-api.herokuapp.com/api/find/artist/song
Example: http://lyric-api.herokuapp.com/api/find/John%20Lennon/Imagine

##Sample Python Code


```python
data = json.load(urllib2.urlopen('http://lyric-api.herokuapp.com/api/find/John%20Lennon/Imagine'))
print(data['lyric'])
print(str(data['lyric']).split())
```


### NOTE: Please do not use this in Production as it is not allowed by the scraped website.
Use this at your own discretion. Lyrics are being scraped from publically available lyrics at lyrics.wikia.com 