# Getting Started

## Prerequisites
- Python 3.9+
- GidronAI API key (request via gidronai.me)

## Installation
```bash
pip install gidronai
```

## Authentication
```python
from gidronai import GidronClient
client = GidronClient(api_key="gai_your_key_here")
```

## Your First Scene
```python
scene = client.scenes.create(
    environment="urban_intersection",
    num_agents=5,
    physics=True,
    frames=100
)
dataset = scene.export(formats=["rgb", "depth", "segmentation"])
dataset.download("./my_first_scene/")
```
