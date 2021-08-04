# Elasticsearch Cheat Sheet
This repo is build for personal use.

But feel free to clone or star it

## Installation on linux
Setup GPG key
```bash
wget -qO - https://artifacts.elastic.co/GPG-KEY-elasticsearch | sudo apt-key add -

sudo apt-get install apt-transport-https

echo "deb https://artifacts.elastic.co/packages/7.x/apt stable main" |

sudo tee -a /etc/apt/sources.list.d/elastic-7.x.list

sudo apt-get update && sudo apt-get install elasticsearch
```

Edit configuration
```bash
sudo nano /etc/elasticsearch/elasticsearch.yml
```

Uncomment the **node.name** line.

Change **network.host** to **0.0.0.0**, **discovery.seed.hosts** to **[“127.0.0.1”]**, and **cluster.initial_master_nodes** to **[“node-1”]**

## Syntax Cheat Sheet
[1. Basic CURL API Sytax](https://github.com/ruanbekker/cheatsheets/tree/master/elasticsearch).


[2. Python Elasticsearch Library Cheat Sheet](https://github.com/ruanbekker/cheatsheets/blob/master/elasticsearch/python-elasticsearch.md#python-library)