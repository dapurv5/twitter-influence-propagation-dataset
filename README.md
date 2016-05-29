# twitter-influence-propagation-dataset
Dataset used in the twitter [influence propagation work](http://arxiv.org/pdf/1603.08981v1.pdf)

```
@article{DBLP:journals/corr/LiXFS16,
    author    = {Shuang Li and
        Yao Xie and
            Mehrdad Farajtabar and
            Le Song},
    title     = {Detecting weak changes in dynamic events over networks},
    journal   = {CoRR},
    volume    = {abs/1603.08981},
    year      = {2016},
    url       = {http://arxiv.org/abs/1603.08981},
    timestamp = {Sat, 02 Apr 2016 11:49:48 +0200},
    biburl    = {http://dblp.uni-trier.de/rec/bib/journals/corr/LiXFS16},
    bibsource = {dblp computer science bibliography, http://dblp.org}
}
```

#### followers/
Contains 50 recent re-tweeters randomly from the account's timeline. These can be thought of as pseudo-followers. Each line in the follower file represents one follower handle for that account.
Each file corresponds to followers of one celebrity.

#### tweets/
The tweets file is a time sorted tsv file. Each line represents one tweet in the network. The first columns stores the time of the tweet. The second column stores the id of the node in the network. The celebrity node is assigned a node id of 1 in each network. The remaining nodes take values from [2-51]. The value in the third column denotes if the tweet was a retweet of the celebrity node. A value of +1 denotes that the tweet was retweet of the celebrity node. (i.e. the node with id=1) and
a negative one denotes that the tweet was not a retweet of the celebrity node.

## Events
The date range for each celebrity node and the important event is presented as follows

##### FLOTUS (Account of Michelle Obama)
- Dates: Jan 1st - Jan 30th, 2016
- Important Event: Birthday on 17th Jan

##### NASA (US Space Agency)
- Dates: Jan 22nd - Feb 2nd, 2016
- Important Event: Challenger space shuttle was launched on 28th January, 1986.

##### jack (account of twitter CEO)
- Dates: Jan 20th - Jan 30th, 2016
- Important Event: Twitter had a mass exodus of employees around Jan 25th

##### whoismrrobot (TV Series Mr Robot)
- Dates: Jan 1st - Jan 20th, 2016
- Important Event: Won golden globe award for best TV series around 10th January

##### ImRaina (account of Indian cricketer)
- Dates: Jan 15th - 4th Feb, 2016
- Important Event: Indian cricket team won a cricket series in Australia around Jan 26th

##### rihanna
- Dates: Dec 20th, 2015 - 4th Feb, 2016
- Important Event: Released a new album called "anti" around Jan 25th

##### MartinShkreli
- Dates: Jan 20th - 9th February, 2016
- Important Event: Court hearing on 4th February

##### ohdaughter
- Dates: Jan 1st - Feb 9th, 2016
- Important Event: New album released on 15th of January

##### isro (Indian space research organization)
- Dates: Jan 1st - Feb 9th, 2016
- Important Event: Jan 20th, successfully launched a satellite into orbit

##### sia (Singer)
- Dates: Jan 10th - Feb 9th, 2016
- Important Event: Jan 29th, 2016, new album released

##### superbowl
- Dates: Feb 1st - Feb 12th, 2016
- Important Event: Superbowl event on Feb 8th, 2016


##### egyptair
- Dates: May 1st - May 28th, 2016
- Important Event: May 19th, egyptair crash 

