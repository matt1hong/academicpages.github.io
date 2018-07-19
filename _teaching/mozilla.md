---
title: "Network Analysis and Visualisation for the Web"
collection: teaching
type: "Tutorial"
permalink: /teaching/mozilla
venue: "Mozilla Festival"
date: 2014-10-25
location: "London, United Kingdom"
---

A tutorial demonstrating techniques to visualize our Facebook networks using the Facebook API and Python.

# [Source code](https://github.com/mhong19414/InteractiveVis)

Generate the network graph
------
1. Download the code from the GitHub repo. Unzip.
2. [Download](apps.facebook.com/netvizz) your network data from the Facebook API. 

    -'Personal network' -> start -> click 'gdf' and Save as...
3. Put this data inside the unzipped folder from GitHub.
4. On command line, go inside the InteractiveVis folder.
5. Make script 'setup.sh' executable:

	`chmod u+x setup.sh`

6. Run the GitHub script to install dependencies: 

	`sudo ./setup.sh`

    -This installs numpy, networkx, and pyparsing. It's important that the networkx installed in your Python is version 1.8.1.
7. Run the Python script to load data, detect communities, and layout nodes: 

	`python main.py`

8. Load up a local server: 

	`python -m SimpleHTTPServer`

9. On Firefox, go to: [http://localhost:8000/network/?config=config_fb.json/](http://localhost:8000/network/?config=config_fb.json/)

Analyze the network graph
------
1. Import the NetworkX library into Python: 

    `import networkx as nx`

2. Import the Counter object: 

    `from collections import Counter`

3. Import graph data into Python: 

	`G = nx.read_gml('facebook.gml')`

4. This will allow you to export the nodes in a useable format, for example:

    ```python
    cent = nx.degree_centrality(G)
    cent = Counter(cent)
    cent.most_common(10)
    ```
    -These functions combined will output the 10 most connected nodes in the graph. There are many other centrality measures, see [the documentation for NetworkX](http://networkx.lanl.gov/index.html)
