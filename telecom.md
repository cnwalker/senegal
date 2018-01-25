# Telecommunications

This page contains more information about the [Fiber Optic Cable System](#fiber-optics), a specific investigation on how [cellular activity might be used to map poverty at high resolution](#mapping-poverty-with-cellular-data), and a [brief history](#history) of telecom in Senegal to give the analysis context.

## Overview
Mobile data is incredibly popular in Senegal. There are 98.68 mobile subscriptions per 100 people[^12], 85% of the total population of Senegal is covered by some kind of mobile network, 20.9% of people are internet users and Telecommunications makes up almost 10% of GDP.

## Mapping Poverty with Cellular Data
Researchers at the Department of Computer Science at SUNY Buffalo found an incredibly strong correlation between [MPI](index.md#what-do-we-mean-by-inequality-and-how-do-we-measure-it) and the communications volume of various regions.

| ![Senegal Cell Towers](./Resources/Telecom/Telecom_Maps/Cell_Towers_Senegal.png) | Cell Towers overlaid with normal MPI |
|:--:|:--:|
| ![Cell Towers and Poverty](./Resources/Telecom/Telecom_Maps/Poverty_and_Cell_Towers.png)| Link and communication volume overlaid with normal MPI |

While the results were excellent in terms mapping the information wealth of the country, the correlation with MPI was not resistant to the removal of Dakar from the dataset. However, when they looked at behavioral metrics like the number of outbound calls, they found a very  

- Paper finds excellent correlation between network centrality and MPI in Senegal

- Dakar has a strong influence on the MPI/Cell-tower correlation, but not when you take into account specific behaviors

- Paper includes calls initiated as key behavioral metric

- Centrality is the importance of a network, in this case determined by flow. Describe Activity, Eigenvector, and PageRank and what each one actually means in practice. (Why Eigenvector is better than Activity, etc.)

- Cell tower work allows for higher granularity poverty maps

- Areas that don't correlate well with MPI do have a fiber optic cable running through them.

- Paper only uses Orange data. Tigo and Expresso have footholds in Dakar and St. Louis, and to a lesser extent in Zinguinchor and Tambacounda. Tigo and Expresso had market share of 23% and 21% respectively as of 2017. The addition of the data from these providers would likely increase the centrality of Dakar, St. Louis, Zinguinchor, and Tambacounda beyond that of the existing model, which would likely have the affect of making the areas not covered by Tigo and Expresso correlate more strongly with a lower MPI.

| Tigo Coverage | Expresso Coverage |
|:--:|:--:|
| ![Cell Towers and Poverty](./Resources/Telecom/Telecom_Maps/Tigo_Map_Large.png)| ![Cell Towers and Poverty](./Resources/Telecom/Telecom_Maps/Expresso_Map_Large.png)|

An constantly updated map with cellular data from all three providers can be found [here](https://www.nperf.com/en/map/SN/-/49.Orange/signal/?ll=14.33651725732605&lg=-14.466950836181695&zoom=7).

### On Centrality
Centrality is a concept from graph theory that is based on determining the "importance" of a node in a network. The best way to think of centrality is, which node is the most popular? If you were to remove a node

- Paper only has calls from within the country, losing out on the large effect that remittances and frequent international calling that may be taking place in rural areas

| Cell Tower Connectivity |  Senegal Fiber |
|:--:|:--:|
| ![Cell Towers and Poverty](./Resources/Telecom/Telecom_Maps/Poverty_and_Cell_Towers.png) | ![Senegal Telecom Cable Map](./Resources/Telecom/Telecom_Maps/senegal_fiber_small.png) |

- Notice that Tambacounda's MPI is high compared to others with similar levels of connectivity. Because many of the cell towers in Senegal are ultimately served by fiber optic cables[^2] it is possible that cellular service is much better in the Tambacounda region because of the proximity to the main fiber lines.


## Fiber Optics
The internet is a series of tubes,[^1] and some of those tubes go through Senegal:

| Senegal | Wider Africa[^3] |
|--|--|
| ![Senegal Telecom Cable Map](./Resources/Telecom/Telecom_Maps/Senegal_Fiber.png) | ![Intra-Africa Optical Fiber Network](./Resources/Telecom/Telecom_Maps/Africa_Fiber.png) |

### What do these maps mean?

The map on the left displays the large underground telecommunications cables that run through Senegal, and the map on the right shows how those cables connect to the rest of Africa and beyond.

The green line that passes from Dakar to Saint Louis and skirts around the border of Louga is the Sonatel fiber optics cable. The red line that goes through Dakar, Saint Louis, Tambacounda, and Ziguinchorr is a x fiber optic line, capable of x output per second.
The dark blue line that comes out of Dakar and cuts through the middle of Senegal is a large optic cable that isn't necessarily fiber (unclear from the diagram)

Fiber optic cables don't only serve wifi connections but are also serve a significant percentage of cell towers. If you're accessing this webpage in Senegal, there is a high probability that the data sent between you and the server went through one of the cables in this diagram.

### What can fiber optic cables tell us?
The Fiber Optic cables are telling because they show where the government of Senegal and large semi-public stakeholders like Sonatel think connectivity to telecommunications services is most important. There are definitely external factors influencing the placement of the cables, like connections with other nations and natural barriers, but the lines go reliably through the major cities of Dakar, Thies, and Saint-Louis, as well as other populous areas like Tambacounda.

Not only do the fiber optic cables tell us where planners think the information centers of the country are, they also can turn areas that are otherwise struggling into information centers as discussed in the case of Zinguinchor

## History
Sonatel was Senegal's state-owned telecom provider until 1997 when it was privatized. The fiber optic cables were laid throughout the late 1990s and early 2000s.

Orange was dominant in Senegal until 2011, when Tigo and Expresso began competing. However even today only urban areas are truly competitive.

[^12]: https://tradingeconomics.com/senegal/international-internet-bandwidth-mbps-wb-data.html
[^1]: U.S Senator Ted Stevens of Alaska
[^2]: Add Intra Africa Cable map citation here
[^3]:http://gu.friends-partners.org/Global_University/Global%20University%20System/List%20Distributions/2012/MTI2312_20120412/Intra-Africa_Fibre_Map_v6-A%20copy.pdf
[^4]:https://www.cia.gov/library/publications/the-world-factbook/fields/2124.html
