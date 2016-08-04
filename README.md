# twitter-influence-propagation-dataset
Dataset used in the twitter [influence propagation work](http://arxiv.org/pdf/1603.08981v1.pdf)

```
@article{DBLP:journals/corr/LiXFS16,
    author    = {Shuang Li and Yao Xie and Mehrdad Farajtabar and Le Song},
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
Contains 50 recent re-tweeters randomly from the account's timeline. These can be thought of as pseudo-followers. Each line in the follower file represents one follower handle for that account. Each file corresponds to followers of one celebrity. Only a select number of handles have their followers in the current version of the dataset.

#### tweets/
The tweets file is a time sorted tsv file. Each line represents one tweet in the network. The first columns stores the time of the tweet. The second column stores the id of the node in the network. The celebrity node is assigned a node id of 1 in each network. The remaining nodes take values from [2-51]. The value in the third column denotes if the tweet was a retweet of the celebrity node. A value of 1 denotes that the tweet was retweet of the celebrity node. (i.e. the node with id=1) and a 0 denotes that the tweet was not a retweet of the celebrity node.

The code used to produce this dataset can be found [here](https://github.com/dapurv5/twitter-influence-propagation-code). I'd like to thank [Tristan Gurtler](https://github.com/tristangurtler) who built upon the initial version of code and did most of the data collection.
