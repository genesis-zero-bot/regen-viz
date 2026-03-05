# regen-viz — 3D Force Graph Visualizations

GitHub Pages repository for interactive 3D network visualizations using [3d-force-graph](https://github.com/vasturiano/3d-force-graph).

## Pages Index

| Page | Description | URL |
|------|-------------|-----|
| Basic | Simple 3D graph with auto-color | [html/basic.html](./html/basic.html) |
| Tree | Tree structure with text labels | [html/tree.html](./html/tree.html) |
| Highlight | Interactive hover highlighting | [html/highlight.html](./html/highlight.html) |
| Curved Links | Curved edge rendering | [html/curved-links.html](./html/curved-links.html) |
| Directional Links | Animated arrows + particles | [html/directional-links.html](./html/directional-links.html) |
| Bloom Effect | Post-processing bloom | [html/bloom-effect.html](./html/bloom-effect.html) |
| Camera Orbit | Auto-rotating camera | [html/camera-orbit.html](./html/camera-orbit.html) |
| Controls Orbit | Orbit camera controls | [html/controls-orbit.html](./html/controls-orbit.html) |
| Controls Fly | Fly-through navigation | [html/controls-fly.html](./html/controls-fly.html) |
| Responsive | Auto-resize on window | [html/responsive.html](./html/responsive.html) |

## Live URLs

Access at: `https://genesis-zero-bot.github.io/regen-viz/html/{filename}.html`

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
    { "id": "node1", "group": 1, "val": 10 },
    { "id": "node2", "group": 2, "val": 15 }
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
regen-viz generate-json --nodes a,b,c --links a-b,b-c

# Create HTML with specific variant
regen-viz create --data mydata.json --variant highlight --name mygraph

# Push to repository
regen-viz publish --name mygraph
```

## Repository Structure

```
regen-viz/
├── README.md
├── _config.yml
├── data/                 # JSON data files
│   └── regen-tribe.json
└── html/                # Generated HTML files
    ├── basic.html
    ├── highlight.html
    └── ...
```

## Based On

- [3d-force-graph](https://github.com/vasturiano/3d-force-graph) by Vasco Asturiano
- CDN: `https://cdn.jsdelivr.net/npm/3d-force-graph`

## Updates

- 2026-03-05: Initial setup with 10 visualization variants
