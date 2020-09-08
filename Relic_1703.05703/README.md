# Relic contours from arxiv:1703.05703

Curves contributed by A. Albert and T. DuPree

The curves are available either as ROOT TGraphs (in the `graphs` directory) or as lists of points in `pickle` files (`lists` directory).

## Naming scheme

The plots in the lepton coupling scenarios are named according to section 2.3.1 of the 2017 DMWG document.

   *	relic_A1.png
   *	relic_A2.png
   * 	relic_V1.png
   *	relic_V2.png 

The plots not fitting this naming scheme correspond to the legacy scenarios with gq = 1.0, which had already been included in the document before:

   * 	relic_axial_gq1.png
   * 	relic_pseudo_gq1.png
   * 	relic_scalar_gq1.png
   *	relic_vector_gq1.png

## Reading example for TGraphs
```python
import ROOT

f = ROOT.TFile("graphs/relic_A1.root")
tmg = ROOT.TMultiGraph()
for tgraph in f.Get("mytlist"):
   tmg.Add(tgraph)
tmg.Draw("A")
```

## Reading example for pickle files
```python
import pickle
from matplotlib import pyplot as plt

with open("lists/relic_A1.pkl","rb") as f:
   contours = pickle.load(f)

for xvalues, yvalues in contours:
   plt.plot(xvalues, yvalues)
```
