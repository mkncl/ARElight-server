# ARElight-server (temporary version for paper review purpose)
![](https://img.shields.io/badge/Python-3.9-brightgreen.svg)

This project represent an accessible version for the 
[ARElight]([https://github.com/nicolay-r/ARElight/tree/v0.25.0](https://github.com/mkncl/ARELight)) system.

<p align="center">
  <img src="https://github.com/mkncl/ARElight-server/blob/main/assets/interface.png?raw=true" alt="metrics_logo"/>
</p>

## Note
Some interaction elements may not work in Safari and Edge. Use Google Chrome for better experience.
Was tested on MPB M3-Pro with Google Chrome v126.

## Installation
```python
pip3 install -r dependecies.txt
```

## Usage

```python
python3 server.py
```

You may follow the UI page at `http://127.0.0.1:8080/`

You can use the following tabs:
1. New Data - Upload a new dataset. The dataset should be a .txt file where each tweet/post/etc. is on a new line. You can select specific parameters and models for data processing.
2. Visualization Settings (Vis) - Configure visualization settings. You can filter vertices by their weight, select opacity, adjust repulsion force, and more.
3. Graph Operations (Operate) - Use this tab to create new datasets by combining others using specific operations.
4. Details - When selecting edges, this tab will show the content of the .txt file related to the selection.

Selection:
1. One click on vertex - show outgoing.
2. 2 clicks on vertex with small delay - show incoming.
3. Click on vertex and then click on other vertex - show edges between these two vertices.

## Layout of the files in output
```
output/
├── force/
    └── ...         // force graphs in JSON.
├── radial/
    └── ...         // radial graphs in JSON.
```
