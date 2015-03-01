The interactome can be visulized here on modern browsers: http://users.wpi.edu/~rosslagoy/interactome.html

Be sure to explore different options for parameters and discuss tradeoffs in your writeup.

I implemented three additional features to the map: highlighting node neighbors, the ability to pin nodes on the svg, and node descriptions on a mouseover. These options allow for user interaction, filtering, and further description of the interactome nodes/links relationships. A descriptive interaction to a visualization like this allows the user to discover and investigate the network interactions. 

A possible tradeoff from combining the node highlight and pinning features is that they are activated by ‘click’ and ‘doublecluck’ events, which can confuse the user when reverting back to the original display; however, I think the filtering and organizing options allowed by these features are more beneficial. I also added a title, description of options, and link to the original published paper, which I think completes the visualization/reference.

A description of your strategy in setting variables.

I studied the provided csv file, then set variables based on the data organization. I realized that the nodes would be called from the BAIT_OFFICIAL_SYMBOL column, and then mapped to the PREY_OFFICIAL_SYMBOL column, creating a linked bait-prey interaction. 
Following d3 force-direct graph examples online, I was able to appropriately set the charge and link distance variables fitting within a common browser size. I knew the force needed to call the graph.nodes and graph.links variables. I made sure I followed all of the TO-DOs to complete the assignment.

How your results compare to Bandyopadhyay et al.’s results.

Figure 3A from Bandyopadhyay et al.’s results is most closely resembled by the visualization developed in this lab. There are clear differences between my and the papers’ original representations in terms of color and layout. The color used in Figure 3A are red for the nodes and grey (no opacity) for the links, with some highlighted links/interactions in red. My nodes are blue and the links are grey with opacity on click events. Additionally, my layout is radial, and the papers’ seems to have some organized direction. This could be replicated through the pinning feature with my map.

Additionally, the authors set a weighting (width) and informational (color) score for the links in Figure 3B-G and Figure 3J-L. These are sub-interactions within the overall interactome, which could be explored in my map through the node-filter and hover options. The nodes in these panels are also different colors and shapes, representing the different kinds of proteins involved in the interactions, providing more description, but could complicate and confuse the novice user by having too many interaction options. Overall, I believe my map successfully represents the main ideas provided by Bandyopadhyay et al.’s original interactome.
