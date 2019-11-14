# vis_icarus
This is for dummies to visualize icarus detector. Bare plotting using plotly, UI as-is from plotly = not great.

### Requirements
* plotly

### How to
```
import plotly.graph_objs as go
from plotly.offline import init_notebook_mode
init_notebook_mode(connected=False)

# Visualization of detector below
from vis_icarus import *
trace,geo = get_trace_icarus(return_geo=True)
fig = go.Figure(trace,layout=icarus_layout3d(geo))
fig.show()
```
See [this notebook example](https://nbviewer.jupyter.org/github/drinkingkazu/vis_icarus/blob/master/notebooks/demo.ipynb).
