# twitter-influence-propagation-dataset
Dataset used in the twitter influence propagation work

#### followers/
Contains 50 recent re-tweeters randomly from the account's timeline. These can be thought of as pseudo-followers. Each line in the follower file represents one follower handle for that account.
Each file corresponds to followers of one celebrity.

#### tweets/
The tweets file is a time sorted tsv file. Each line represents one tweet in the network. The first columns stores the time of the tweet. The second column stores the id of the node in the network. The celebrity node is assigned a node id of 1 in each network. The remaining nodes take values from [1-50]. The value in the third column denotes if the tweet was a retweet of the celebrity node. A value of +1 denotes that the tweet was retweet of the celebrity node. (i.e. the node with id=1) and
a negative one denotes that the tweet was not a retweet of the celebrity node.
