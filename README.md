# sopel-lowtechnews
\#lowtech news module for Sopel IRC bot

# Installation
Tested on Ubuntu 16.04 LTS. Requires python 3.5

```bash
sudo pip3 install sopel requests
```

# Usage
Check repository out to the Sopel repositories directory, symlink into enabled 

Retrieve a value from [https://news.lowtech.io](#lowtech news) using:
```
.n #800000
```

Perform a search for content
```
.n content search
```

Find trending content within the last 24 hours and show 10 words
```
.trending 24 10
```

# Testing

```bash
$ python3 lowtechnews.py 
Looking up '424347':
Successfully loaded #424347
         <ApiResponse 200:'OK' {'results': [{'domain': 'www.twitch.tv', 'date_added': '2017-08-19 03:45:08', 'hash': 't10f6MWNdqJ...


Looking up 'candy crush':
Successfully loaded search results with 7 search results
         <ApiResponse 200:'OK' {'results': [{'date_added': '2017-10-02T14:58:51Z', 'title': 'Are We Being Candy Crushed at Work?'...


Looking up trending words over the last 48 hours and requesting 15 words
Successfully loaded 15 trending words:'
         after, trump, us, new, why, youtube, from, 2018, video, south, has, mudslides, ces, california, about
```
