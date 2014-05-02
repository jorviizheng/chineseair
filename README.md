# [Chinese Air](http://kopf.github.com/chineseair/)

Graphing air quality readings from several major Chinese centers: Beijing, Shanghai, Guangzhou, Chengdu & Shenyang.

This is the source code of the project which is viewable at http://kopf.github.com/chineseair/

These files may be of interest:

* `chineseair/updater.py`, which scrapes the data from web feeds
* `chineseair/google.py`, the interface for the Google Fusion Tables API
* `chineseair/process_historical_data.py`, which processes full historical records (see [here](http://www.stateair.net/web/historical/1/1.html) for an example) published on stateair.net

## Why is this repo so huge? Why so many commits?

I put this project together in an evening. In its first incarnation, the `updater.py` script would simply scrape twitter and save any new data to a json file in this repo, commit and push. This json file would then be loaded when the user visited the project webpage.

It was a very quick-and-dirty solution, and led to the tens of thousands of commits (and the huge repo size) today. I would like to clean up the git history, but I'm reluctant to, since people have already forked this repo. 
