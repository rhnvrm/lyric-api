# lyric-api
API that returns lyrics after searching on lyrics.wikia.com based on Artist and Song.

## Deploy on Heroku

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

Deployed at: 
https://lyric-api.herokuapp.com/api/ <del>and
http://128.199.199.233:8081/api/</del>

Usage: https://lyric-api.herokuapp.com/api/find/artist/song<br>
Example: http://lyric-api.herokuapp.com/api/find/John%20Lennon/Imagine

## Sample Python Code


```python
data = json.load(urllib2.urlopen('http://lyric-api.herokuapp.com/api/find/John%20Lennon/Imagine'))
print(data['lyric'])
print(str(data['lyric']).split())
```


### NOTE: Please do not use this in Production as it is not allowed by the scraped website.
Use this at your own discretion. Lyrics are being scraped from publically available lyrics at lyrics.wikia.com 

## [lyric-get](https://github.com/rhnvrm/lyric-api/blob/master/lyric-get/)

[![npm version](https://badge.fury.io/js/lyric-get.svg)](https://badge.fury.io/js/lyric-get)

Module for fetching lyrics from lyrics.wikia.com using artist name and song.

## Installation

`npm install lyric-get`

## Usage

```nodejs
var l = require("lyric-get");

l.get("John Lennon", "Imagine", function(err, res){
    if(err){
        console.log(err);
    }
    else{
        console.log(res);
    }
});
```
