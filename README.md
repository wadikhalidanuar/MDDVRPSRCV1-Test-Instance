# VRP-Test-Instance

Thank you for your interest in the proposed test instances

the proposed test instance is aimed towards VRP problem that addressed in particular < TO BE ADDED LATER TO PROTECT NOVELTY RESEARCH >

The instance problem consists of road network mapped in eucledean distance where the road capacity of edges, depots, shelters, and connecting nodes coordinates as well as demand of shelters are fixed.

Meanwhile the "damage" file addressed the damage value of edges within the network due to an event triggered from a single point.

******************************************************************************************************************************************************************
This proposed instance is made possible through the author: Anuar, Wadi Khalid, and his PhD research supervisor: Lai Soon, Lee, as well as the contributing instituition: Universiti Utara Malaysia (affiliated to author) & Universiti Putra Malaysia (affiliated to research instituition)

We humbly request those who find the proposed instances beneficial for their research work to also acknowledge us as the original contributor to these Test Instances in their publications and projects.

Heres how you can cite this repository:

  for now:

    Anuar, Wadi Khalid, Lai Soon, Lee, (2021)VRP-Test-Instance[Source Code].https://github.com/wadikhalidanuar/VRP-Test-Instance
    
  when paper with first use of instance is published:
  
    bibtex cite of the paper

******************************************************************************************************************************************************************

This instances can be downloaded through the zip files:
1) LOAD_INSTANCE TO GITHUB.zip

Each instance is an excel file containing:
1) number of depots, connecting nodes and shelters + (optional fix vehicle number under "M")
2) the coordinate of each node (depot, shelter, connecting nodes)
3) the road capacity of edges in the network
4) the demands for each shelters
5) road network

This "damage" data associated with the instances can be downloaded through the zip files:
1) LOAD_DAMAGE TO GITHUB.zip

Each damage file is an excel file containing:
1) edges with damage value
2) coordinate of disaster epicenter (e.g earthquake)

******************************************************************************************************************************************************************
A python file served as an example is provided to extract the instance and damage data:
1) LOAD_INTS_DAMG_V2.py

The output of these python code is:
1) cost or distance matrix
2) time travel matrix
3) road capacity matrix
4) edges
5) edges-> damage value dictionary


the cost matrix is proportional to the distance calculated based on eucledean distance

the time matrix is computed based on the assumption that vehicle moves under constant velocity 90km/h and delay due to the damage value of each edges.

*******************************************************************************************************************************************************************
REQUIREMENTS
*******************************************************************************************************************************************************************
1) Python 2.7. The python code to load the test instance and damage file into python is tested with python 2.7. It is possible to convert the code to python 3. some syntax changes is advised
2) microsoft excel
3) zip file extraction tools

*******************************************************************************************************************************************************************
INSTRUCTIONS
*******************************************************************************************************************************************************************

1) Download:
(a) LOAD_INSTANCE TO GITHUB.zip
(b) LOAD_DAMAGE TO GITHUB.zip
(c) LOAD_INTS_DAMG_V2.py

2) unpack (a) in a different folder. note the path to folder where (a) is unpacked
3) unpack (b) in a different folder. note the path to folder where (b) is unpacked

4) open LOAD_INTS_DAMG_V2.py with python 2.7 

5) copy the path (a) in the python code to load instance files
6) copy the path (b) in the python code to load "damage" files

7) run the python code
