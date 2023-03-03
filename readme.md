## GeoGraphVis Experiments

There are two sets of datasets. 
Dataset1 is the real-world data which represent a network of expertise with infectious disease related expertise. This expert network is used by a non-profit organization Direct Relief to search and locate expert in a disaster response scenario. 

There are two files under the folder of dataset1:
- `DR_sim20.csv`
- `expert_loc.json`

The CSV file contains the similarity scores between each expert (node) pair. The scores
are maintained in a N by N matrix (N is the number of nodes). The CSV header indicates the order of experts in each column and row. The `expert_loc.json` contains location information for each expert's affiliation. 

Dataset2 is a simulated dataset containing a larger graph with international presence. The folder contains two files:
- `sim_uw0.45_ub0.3_s0.1.csv`
- `international_placenames2.json`

The CSV file has the same structure as that in the first dataset. The JSON file contains the geolocation and other attributes of each node mentioned in the above CSV file. 

In the CSV file name of simulated data, the number followed by "uw" indicates the mean similarity score (a hypothetical value used to generate the simulation data) between nodes belonging to the same semantic cluster. The number followed by "ub" indicates the mean similarity score (another hypothetical value) between nodes belonging to different semantic clusters. The number followed by "s" indicates the standard deviation of the generated similarity scores. See more detail about data generation in the data simulation section of the paper.

The `exp.html` contains javascript code for loading the datasets for visualization. 

The live GeoGraphVis interface can also be found through this link: [http://cici.lab.asu.edu/kwg/](http://cici.lab.asu.edu/kwg/)

