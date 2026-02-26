# Dijkstra-s-Algorithm-Guangzhou-Metro-Simulation
Simulating Guangzhou’s metro system using Dijkstra’s algorithm to determine the shortest path between two stations. 

## Project 1 Metro Simulation ##
Sunny Chen

10/25/2024

### Introduction: ###

Urban transport systems, such as metros can provide efficient mobility for densely populated areas. Having access to reliable public transportation is not only for convenience but it can also have a positive impact on promoting social equity. Public transportation has benefits for those who cannot afford private vehicles and people with disabilities, such as individuals who are visually impaired. It allows them to access essential services like healthcare, education, and employment. Without reliable transit options, these groups face significant challenges and limitations to opportunities and services that many take for granted. A well-optimized public transportation system reduces dependence on cars and promotes sustainable development which builds livable, inclusive communities. 
There are many applications that are used to recommend the most efficient travel paths for passengers and graph theory serves as the foundation for these systems. Dijkstra’s algorithm is efficient when it comes to finding the shortest path in a graph that contains positive weights, making this algorithm very applicable for determining the most efficient route when traveling using a metro system. 

### Project Specification ###
We will be simulating Guangzhou’s metro system using Dijkstra’s algorithm to determine the shortest path between two stations. A metro network with 23 stations (S1-S23) will be created and the edges will be the distance between the stations. The graph will be an undirected, weighted graph. We will use Dijkstra’s algorithm to allow a user to select a starting point and a destination. Paths between the nodes will be undirected meaning that passengers can travel in either direction between two adjacent stations. The edges will have positive weights representing the distance between stations in kilometers. The primary goal is to be able to use Dijkstra’s algorithm to determine the shortest path between stations and allow a user to travel to their destination efficiently. The user will be able to input the graph, starting point, and destination and receive the shortest path and travel distance along the nodes. We will test various paths and ensure it works correctly for different starting points and destinations. 

### Implementation ###
We first create an adjacency list which will be used to form our graph with nodes and edges. The adjacency list will provide us with the nodes, the neighboring nodes, and the distance between adjacent nodes. The graph that is created will be ‘G’ which is then used as an input for the function. 
The function used that implements Dijkstra’s algorithm, outputs the shortest path from the source to the destination as well as the total distance traveled. In our first example, we use ‘S1’ as the source and ‘S21’ as the destination. The function takes three inputs, G for the graph, the source, and the destination. Our output using S1 and S21 gives us a total travel distance of 12km and the shortest path by traveling along the following nodes: ['S1', 'S2', 'S3', 'S7', 'S6', 'S20', 'S21']. 
