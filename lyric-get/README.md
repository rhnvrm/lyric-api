#lyric-get

[![npm version](https://badge.fury.io/js/lyric-get.svg)](https://badge.fury.io/js/lyric-get)

module for fetching lyrics from lyrics.wikia.com using artist name and song.

#Installation

`npm install lyric-get`

#Usage

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