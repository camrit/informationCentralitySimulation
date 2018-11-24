 ## WHAT IS IT?

This is a simulation of network flow through Parallel Duplication through four kinds of flows: Geodescis, Paths, Trials and Walks

## HOW IT WORKS

The Turtels are the nodes that has three attribes
1) Information (the information is incremented as the node is passed)
2) Node Passed? (boolean: green if not and red if it has been passed)
3) temp-count (not used for parallel duplication)

While the links (the edges) have the following three attributes
1) information-flow (this variable is incremented everytime the link is passed)
2) links-passed? (boolean variable)
3) temp-flow (not used for parallel duplication)

For each type of network flow; namely: walk, trial, path and geodesic we simulate the flow from a source node (we iterate through all the nodes) to a target node a 1000 times and then compute the average node statistics:

Pseudo Code:

For i = 1 to 1000 (Independent Trials){
	For j = 1 to n (nodes){  //For each source node
		For k = 1 to n { //For each target node

			Simulate flow i from j to k (when k is reached 'found' = True)
		}
	}
	Compute node statistics for this trial
}
Average node statistics and compare with centrality measures


## HOW TO USE IT

First one needs to set up the network and then choose one particular network flow

## THINGS TO NOTICE

(suggested things for the user to notice while running the model)

## THINGS TO TRY

(suggested things for the user to try to do (move sliders, switches, etc.) with the model)

## EXTENDING THE MODEL

(suggested things to add or change in the Code tab to make the model more complicated, detailed, accurate, etc.)

## NETLOGO FEATURES

(interesting or unusual features of NetLogo that the model uses, particularly in the Code tab; or where workarounds were needed for missing features)

## RELATED MODELS

(models in the NetLogo Models Library and elsewhere which are of related interest)

