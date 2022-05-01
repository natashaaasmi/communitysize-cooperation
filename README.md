# communitysize-cooperation

The intent of this project was to evolve spatially-structured communities that favor cooperative strategies over selfish ones. Modeling was done in Python Mesa, an agent-based modeling framework. 
There were two initial phenotypes: 
  1) Cooperator (C). Adds resources to the community pool, directly transfers resources to other low-resource individuals. Generally acts in the best interest of the community. The majority of individuals within the community have the C phenotype.
  2) Defector (D). Does not add to the community pool or directly transfer resources to other individuals. A constant small fraction of individuals at each community size have the D phenotype. If a C individual directly transfers resources to a D individual, it is turned into a neutral (N) individual, which cannot add to the community pool. 

# For each model:
Cooperation was measured with a proxy 'community pool' of resources that C individuals contributed to. Ratios of C to D individuals before the model was run and after the model was run -- this is an easy way to test the success of cooperative vs selfish strategies. 

# Evolving models:
Individual models were created with random values for grid size and number of agents. A stable ratio of the total number of agents were designated cooperators/defectors. Fitness values were assigned to each individual model; these fitness values rewarded proxies for cooperation and punished individual communities that favored selfish strategies. 

# Results: 
I'm currently stuck on some errors in the evolving models segment, but wanted to upload what I had for the model right now and hopefully fix those issues later. However, initial results (without evolution) indicate that according to the rules I made, defection is always a favorable strategy. For example, I tested a randomly generated population of 100 model communities. Each one of those communities had a high ratio of defectors/cooperators and a community pool size of 0. 

#Visualization:
Once the errors are fixed there will be an interactive visualization attached to each model

#Extension:
This project will eventually serve as initial supporting research for decision-making in a larger project called Halogen (whitepaper linked in this repository); however, the model will need to be much more refined and accurate for that to work. 
