Response to Strano



Notes from reading

rising global connectivity = spread of disease and drug resistance, shorter distance movements over roads important for spread in low income communities
roads directly relate to population densities and travel and connectivity
general approach road netword studying: model road as a networka and study topological structure (environmental and social impact).
easier to reach goals in less connected more isolated areas

methods for identifying and mapping road connectivity communitites

ARN: dataset of primary and secondary roads
  primal road network : roads are links, road junctions are nodes
  freq dist of degree of nodes (number of roads (links) connected to each node
  
detecting communities: human displaceement in urban networks guided by straight lines
  community detection pipeline: converts primal road network to dual network (links are nodes, street junction link btwn nodes via straightness and contiguity of roads)
   THEN community detection with modularity optimization algorithm
    algorithm looks for edge with longest road, then node created and look for seconf longest road, connect nodes if roads intersect. 
    modularity-based algorithm to detect communitites
    
modeled communities align with hiv subtypes and disease spread!!
    
shows connectivity rarely aligns with national borders.
