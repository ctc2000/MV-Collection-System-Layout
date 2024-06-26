# MV Collection System Mapping

This tool supports the initial design process for MV Collection Systems of wind farms. 

### Input
Coordinates of a wind turbine generator (WTG) array and substation in CSV format.

### Output
KML layout with load and turbine location data embedded.

### Outcomes
1. Initial KML file for MV Collection System design. Edit the cable routes further in any GIS tool to avoid obstacles, crossings, and restricted land.
2. Automated cable sizing and cable schedule creation.


# Capacitated Minimum Spanning Tree Problem

### Problem Statement
An optimal WTG network should theoretically be designed as a capacitated minimum spanning tree (CMST). This is a minimum spanning tree with the following attributes:
- A root node, which is the central hub of the network
- The number of nodes on branches of trees must not exceed a capacity value

The CMST is applied to networking problems in which balanced sub-networks are connected to a central hub: computer networking and communications, transportation routes, as well as cable trenching. Finding the CMST is an NP-hard combinatorial optimization problem. 

An additional requirement for terrestrial wind farms is to eliminate all crossing paths so that cable trenching is feasible. While heuristics exist to find suboptimal CMST's, these do not satisfy the land-based constraints for practical WTG network design.

### Solution
Due to land control, roads, wetlands, buildings, and further geotechnical constraints, terrestrial MV collection system layouts require a thoughtful design process. This tool provides clustering and MST visualizations to guide the layout. Then, user input of WTG groups allows flexibility for project-specific constraints. Finally, MST algorithms are used to connect each group of WTG's to the substation, and a KML file is produced.

# Sample Workflow

### Turbine and Substation Coordinates (CSV)

### Output KML

### Adjust Cable Routes & Add Junction Boxes

### Automated Cable Schedule Creation

### MV Collection System Single Line Diagram

