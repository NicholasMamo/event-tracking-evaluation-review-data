# The Myth of Reproducibility: A Review of Event Tracking Evaluations on Twitter

This repository stores the data used in the paper _The Myth of Reproducibility: A Review of Event Tracking Evaluations on Twitter_.
In compliance with Twitter's data-sharing policy, we only share tweet IDs but provide a tool with which to download the original tweets.
This repository is structured as follows:

- The `config` directory contains an example configuration file.
  Copy this file into `conf.py` if you intend to re-download the data.
- The `data` directory contains the tweet IDs and metadata files with information about how we collected the original corpora.
  We do not include [Waseem and Hovy (2016)'s](https://github.com/zeeraktalat/hatespeech) and [Founta et al. (2018)'s](https://github.com/ENCASEH2020/hatespeech-twitter) datasets, which the authors made available in the original repositories.
- The `downloaded` directory contains the tweet IDs and metadata files with information about how we re-downloaded the corpora.
- The `lib` directory contains functions that the download tool uses to re-download corpora.
- The `tools` directory contains the `download.py` tool, which you can use to download the original tweets from the provided IDs.
  Use the `download.py` tool with the `-h/--help` parameter to see usage instructions.
Note that to use the download tool, you require Python 3 and the [Tweepy library](https://github.com/tweepy/tweepy) installed.
