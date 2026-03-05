# regen-viz — 3D Force Graph Visualizations

GitHub Pages repository for interactive 3D network visualizations using [3d-force-graph](https://github.com/vasturiano/3d-force-graph).

## Pages Index

| Page | Description | Data Source |
|------|-------------|-------------|
| [basic](./html/basic.html) | Basic 3D graph | Generated |
| [tree](./html/tree.html) | Tree structure | Generated |
| [highlight](./html/highlight.html) | Interactive highlighting | Generated |
| [text-nodes](./html/text-nodes.html) | Nodes with labels | miserables.json |
| [img-nodes](./html/img-nodes.html) | Image nodes | Generated |
| [curved-links](./html/curved-links.html) | Curved edges | Generated |
| [directional-links](./html/directional-links.html) | Directional arrows | Generated |
| [bloom-effect](./html/bloom-effect.html) | Post-processing bloom | Generated |
| [camera-orbit](./html/camera-orbit.html) | Auto-orbiting camera | Generated |
| [controls-fly](./html/controls-fly.html) | Fly controls | Generated |
| [controls-orbit](./html/controls-orbit.html) | Orbit controls | Generated |

## Quick Start

### Add a new visualization

1. Create JSON data in `data/` folder
2. Create HTML in `html/` folder
3. Commit and push
4. Access at: `https://genesis-zero-bot.github.io/regen-viz/html/your-file.html`

## Data Format

```json
{
  "nodes": [
    { "id": "node1", "group": 1, "label": "Node 1" },
    { "id": "node2", "group": 2, "label": "Node 2" }
  ],
  "links": [
    { "source": "node1", "target": "node2" }
  ]
}
```

## Skill Usage

Use the `regen-viz` skill to generate visualizations:

```
# Generate graph from data
regen-viz generate --data '{"nodes":[...], "links":[...]}'

# Create HTML with specific variant
regen-viz create --variant highlight --name my-graph

# Push to repository
regen-viz publish --name my-graph
```

## Repository Structure

```
regen-viz/
├── README.md
├── _config.yml
├── data/                 # JSON data files
│   └── *.json
└── html/                # Generated HTML files
    └── *.html
```

## Based On

- [3d-force-graph](https://github.com/vasturiano/3d-force-graph) by Vasco Asturiano
- CDN: `https://cdn.jsdelivr.net/npm/3d-force-graph`

## Updates

- 2026-03-05: Initial setup with 11 visualization variants
