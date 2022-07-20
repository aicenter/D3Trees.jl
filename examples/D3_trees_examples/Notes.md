# D3 tree stuff

There is no simple API way of dynamically adding nodes to D3 hierarchy:

- Issue: <https://github.com/d3/d3-hierarchy/issues/139>
- Question: <https://github.com/d3/d3-hierarchy/issues/139>

So to migrate to d3 above version 3, some changes are required:

- when adding nodes with fetch, either:
  - update all parent nodes "height" as well as other params (probably preffered)
  - recalculate `hierarchy` for the whole data structure

This will probably not be too difficult, but I need to figure out some easier workflow with javascript. Its too slow to figure out what's going on when editing html files.

## Pannable tree

Example of d3 tree in v3 with pannable tree, something that could be useful here:

- page: <http://bl.ocks.org/robschmuecker/7880033>

