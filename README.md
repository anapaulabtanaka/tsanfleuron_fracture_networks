[![DOI](https://zenodo.org/badge/1008321304.svg)](https://doi.org/10.5281/zenodo.15739430)

# Tsanfleuron fracture networks as graphs
Data set, interpretations, measurements, analysis, and examples. 
<br>
<img src="./cover/tsan_frac_net.png" alt="tsan_networks">

<br/>

This repository is associated with my phD research, abstract and submitted paper:

<br/>

**1) Abstract for World Groundwater Congress (IAH2024): Graph-based modeling of fractures in the Tsanfleuron karst aquifer system**

Ana Paula Burgoa Tanaka <sup>*</sup>, Philippe Renard, Jefter Natan de Moraes Caldeira, Xiao Xia Liang, Celia Trunz, and Julien Straubhaar


<br/>

**2) Paper submitted: Graph-based fracture network analysis to integrate structural geology properties and identify preferential flow pathways in the aquifer system of Tsanfleuron, Swiss Alps**

Ana Paula Burgoa Tanaka <sup>*</sup>, Philippe Renard, Jefter Natan de Moraes Caldeira, Celia Trunz

\* corresponding author: ana.burgoa@unine.ch

<br/>

## Data description

### Files

In the "data/dataframe" folder, you will find:

- The daframe with all fractures attitudes measured in the 2D interpretation, 3D point cloud interpretation, and field (outcrops and scanline) 
  - Filename: `tsan_structural_all.csv`
 
In the "data/graphs" folder, you will find:

- The fracture network as graphs
  - Filename: `tsan_fracgraph.pickle`

In the "data/shapefile" folder, you will find:

- The fracture network 2D interpretation
  - Filename: `tsan_fractures.shp`

- The fracture network separated in sets
  - Filename: `NS_line.shp`
  - Filename: `NESW_line.shp`
  - Filename: `EW_line.shp`
  - Filename: `NWSE_line.shp`

In the "data/stereo" folder, you will find:

- The fracture attitudes measurements separeted according to the acquisition
  - Filename: `stereo_cloudpoint.txt`
  - Filename: `tsan_all_azimuths.txt`
  - Filename: `tsan_all_dem.txt`
  - Filename: `tsan_terrain_all.txt`

- The file to plot a steronet using openstereo (https://github.com/spamlab-iee/os/releases/tag/v2.0b12)
  - Filename: `tsan_field_cloud_dem.openstereo`

 In the "data/tensor" folder, you will find:
 
- The project to do the kinematic analysis and paleostress tensor inversion with WinTENSOR (http://damiendelvaux.be/Tensor/WinTensor/win-tensor.html)
  - Filename: `tsan_kine_paleostress.wtd`

## Dependencies

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install the following packages.

```bash
pip install numpy matplotlib pandas scipy geopandas shapely networkx pickle math jupyter-notebook plotly astropy pwlf fracability karstnet random cv2
```
                
## Examples

Jupyter notebook examples to characterize the networks, analyze, and export:

- Ex01_Fracture_geometries.ipynb
- Ex02_Fracture_power_law.ipynb
- Ex03_Fitting_length_distribution_with_fracability.ipynb
- Ex04_Fracture_density.ipynb
- Ex05_Fracture_networks_graphs_-_graph_and_geometries.ipynb
- Ex06_Fracture_networks_graphs_-_topologies.ipynb
- Ex07_Fracture_networks_graphs_-_topology_with_fracability.ipynb
- Ex08_Fracture_networks_graphs_-_centralities_and_percolation.ipynb
- Ex09_Exporting_networks_graphs.ipynb
