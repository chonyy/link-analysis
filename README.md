<p align=center>
    <img src="img/graph_4.png">
</p>

<p align=center>
    <a target="_blank" href="https://travis-ci.com/chonyy/AI-basketball-analysis" title="Build Status"><img src="https://travis-ci.com/chonyy/AI-basketball-analysis.svg?branch=master"></a>
    <a target="_blank" href="#" title="language count"><img src="https://img.shields.io/github/languages/count/chonyy/PageRank-HITS-SimRank"></a>
    <a target="_blank" href="#" title="top language"><img src="https://img.shields.io/github/languages/top/chonyy/PageRank-HITS-SimRank?color=orange"></a>
    <a target="_blank" href="https://opensource.org/licenses/MIT" title="License: MIT"><img src="https://img.shields.io/badge/License-MIT-blue.svg"></a>
    <a target="_blank" href="#" title="repo size"><img src="https://img.shields.io/github/repo-size/chonyy/PageRank-HITS-SimRank"></a>
    <a target="_blank" href="http://makeapullrequest.com" title="PRs Welcome"><img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg"></a>
</p>

> Python implementation of famous link analysis algorithms.

- HITS Algorithm
- PageRank Algorithm
- SimRank Algorithm

## How to use

Get a copy of this repo using git clone
```
git clone https://github.com/chonyy/PageRank-HITS-SimRank.git
```

Run the program with dataset provided and **default** values for *damping_factor* = 0.15, *decay_factor* = 0.9 and *iteration* = 100

```
python main.py -f 'dataset/graph_1.txt'
```

Run program with dataset and cusotm parameters

```
python main.py --input_file 'dataset/graph_1.txt' --damping_factor 0.15 --decay_factor 0.9 --iteration 500
```

## Result

### Output on console

<p align=center>
    <img src="img/output.png">
</p>

The order of the result follows the order of the node value. For example, `1, 2, 5, 7`.

### Output to files in result folder

<p align=center>
    <img src="img/result.png">
</p>

A new folder with the name same with the graph will be created in the result directory. Four txt files will be created to store the value printed on the console.

- graph_HITS_authority.txt
- graph_HITS_hub.txt
- graph_PageRank.txt
- graph_SimRank.txt