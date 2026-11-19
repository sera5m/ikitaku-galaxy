# ikitaku-galaxy

3D / 2D force-graph of concept hierarchies and Toplethos neuron links.
Inspired by [obsidian-galaxy](https://github.com/agentage/obsidian-galaxy)
(three.js + 3d-force-graph). Standalone page, not an Obsidian plugin,
so a human or a model can edit the graph as JSON.

Open `index.html`. Keyword search and rank filter are in the bar.
The 2D checkbox drops to two dimensions.

## Graph shape

```json
{
  "nodes": [{ "id": "cycle-add", "rank": 4, "kind": "form", "label": "cycle-add" }],
  "links": [{ "source": "cycle-add", "target": "cycle", "rel": "outer" }]
}
```

Rank 5 is a platonic verb. Rank 4 is a composition. Rank 3 is a word
mapped onto a form. Edges carry the relation (`outer`, `inner`,
`maps`, `sign`).

The sample graph shows `cycle-add` and `add-cycle` as different nodes
with different outer/inner edges. That is the non-commutative check.
