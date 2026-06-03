# chart-waffle

The waffle chart data is procedurally generated in JavaScript (100 squares per group with
status assigned based on the critically-endangered percentage from vertebrate_detail.json).
The Vega-Lite spec is embedded in index.html and references this computed dataset.

Source data: data/vertebrate_detail.json
Groups: Fish (35.4% CE), Frogs (36.7% CE), Reptiles (26.7% CE)
