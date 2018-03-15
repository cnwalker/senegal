[Click here to download a video game where you live as a farmer in the colonial senegambia](Resources/Senegambian_Trails_Final.zip)

# The Role of Utilities
This site exists to investigate whether access to and physical placement of public utilities, particularly [water](water.md), [electricity](electricity.md), and [telecommunications](telecom.md) can help us better understand poverty in Senegal.

| ![Cellular Activity](./Resources/Telecom/Telecom_Maps/Poverty_and_Cell_Towers.png) | ![MPI map of Senegal](./Resources/Electricity/Senegal_Electric_Grid.jpg) | ![MPI map of Senegal](./Resources/Water/Senegal_Hydrogeology.png)|
|:--:|:--:|:--:|
| *Cellular activity* | *Electric Grid* | *Hydrogeology Map of Senegal* |

## Abstract and Findings
Each of the three utilities have different lessons to teach us about inequality in the republic of Senegal.

[Water](water.md) helps illustrate the complexity of understanding when progress is made in an area. As demonstrated by the increase in access of water in rural areas in Senegal, but neglect of the quality.

[Telecommunications](telecom.md) and [electricity](electricity.md) demonstrate where information-based wealth is and may give unprecedented granularity for understanding and mapping poverty. Telecom also demonstrates how infrastructure can influence conditions in regions in Senegal in addition to helping us study them.

The Senegalese electric grid, originally created to provide lighting on public roads, now serves 55% of the people of Senegal. The distribution of access to electricity is much lower in rural areas, where only 26% of people have access to electricity.[^0]

The correlation between access to electricity and poverty is well-captured in the MPI metric, however access to electricity is also a prerequisite for access to telecommunications.

One of the most striking insights from looking at telecommunications in Senegal is the capacity to train models to produce higher resolution poverty maps than were previously thought possible. By using cellular communication data from Orange, researchers at SUNY Buffalo were able to train a model to predict the [MPI](#what-do-we-mean-by-inequality-and-how-do-we-measure-it) - a widely used metric for quantifying poverty - of regions in Senegal at much higher resolution than was previously possible.

| Normal MPI map | Cellular Model MPI Map[^8] |
|:--:|:--:|
| ![MPI map of Senegal](./Resources/Livelihood_Zones/senegal_mpi_map.png)| ![Cellular poverty map](./Resources/Telecom/Telecom_Maps/High_Granularity_Poverty_Map.png) |

There are a number of potential issues with the model that are discussed further in the [telecom](telecom.md) section, but the researchers have recently received funding from the Bill and Melinda Gates foundation that will hopefully allow them to correct issues and improve the resolution of the map even further.[^12]

## What do we mean by inequality, and how do we measure it?
From access to public services like healthcare to educational attainment and income disparity, there are a number of ways to measure poverty and inequality. The metric used to measure poverty for this project is [MPI](https://en.wikipedia.org/wiki/Multidimensional_Poverty_Index), which is a widely-used metric designed to measure acute poverty.[^1] Higher MPI indicates greater poverty and lower access to resources, while lower MPI indicates the inverse.

Inequality between the wealthy and the middle class in Senegal may also have an interesting relationship with the placement of and access to utilities, but it is very difficult to make statements about actual happiness and life satisfaction after a certain income level, while there is good evidence to support that lack of access to basic needs like healthcare, education, and sanitation cause people to report lower life satisfaction and greater emotional pain when stressful situations occur.[^3]

One of the great advantages of MPI is that it is designed to be "robust to decomposition within the relevant sub-groups of populations like urban vs. rural, geographic regions, ethnicity, and gender", and the data it depends on is available with high fidelity in Senegal[^4]. It is important to note however that the calculation of MPI is partially based on indicators of access to water and electricity, which may bias some of the findings on this site to have a stronger correlation with MPI than if those factors were controlled for. Fortunately, access to water and electricity alone make up relatively small portions of the MPI calculation[^5]


## Footnotes
[^8]: https://arxiv.org/abs/1506.03401
[^12]: http://blog.weebi.com/a-mapping-with-a-meaning/
[^0]: https://www.usaid.gov/powerafrica/senegal
[^1]: http://blog.weebi.com/a-mapping-with-a-meaning/
[^2]: http://www.ophi.org.uk/wp-content/uploads/MPI_2011_Methodology_Note_4-11-2011_1500.pdf?cda6c1
[^3]: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2944762/
[^4]: https://arxiv.org/abs/1506.03401, page 2
[^5]: Electricity and water make up (1/18th) of the MPI calculation respectively, while factors like access to education make up (1/6th)
