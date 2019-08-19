# RelicDensityCurves

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3250544.svg)](https://zenodo.org/badge/DOI/10.5281/zenodo.3250544.svg)

DM relic density curves for various simplified models of dark matter

When using those curves, please cite: 

Recommendations of the LHC Dark Matter Working Group: Comparing LHC searches for heavy mediators of dark matter production in visible and invisible decay channels
https://arxiv.org/abs/1703.05703

Dark Matter Benchmark Models for Early LHC Run-2 Searches: Report of the ATLAS/CMS Dark Matter Forum
https://arxiv.org/abs/1507.00966

[instructions by A. Albert]

Each of the independent curves is saved as a separate TGraph in a TList. It appears that when you simply double click a TList in the ROOT browser, it will only draw one of the graphs in the list.
To get all graphs, please iterate over the list. See the code example at https://gist.github.com/AndreasAlbert/03108fc24e706d38a88b3988346de308.
