# Facebook_page_analysis
A set of data (147MB) comprising Facebook pages information such as likes, talking about count and check-ins are analysed for food and beverages companies.

The data are filtered based on top 250 restaurant chain in US ('https://www.fsdbco.com/top-250-restaurant-chains-us-2019/').
51 Facebook pages were idenfified related to the filter.

**Table 1:** Top 5 most liked page in the dataset for food & beverage (USA) 
| Index | Facebook page name | Facebook likes | 
| --- | --- | --- |
| 1 | McDonalds | 78,045,025 |
| 2 | McDonaldsUS | 78,015,575 |
| 3 | KFC | 51,635,735 |
| 4 | Starbucks | 37,189,939 |
| 5 | PizzaHut | 31,513,432 |

**Table 2:** Top 5 least liked page in the dataset for food & beverage (USA) 
| Index | Facebook page name | Facebook likes | 
| --- | --- | --- |
| 1 | PolloTropical | 176,449 |
| 2 | flemings | 122,103 |
| 3 | GrandLuxCafe | 81,442 |
| 4 | EddieVsPrimeSeafood | 74,770 |
| 5 | Lubys | 35,593 |

**Table 3:** Mean, median and standard deviation for food & beverage (USA) 
| Index | Facebook likes |
| --- | --- |
| median | 1.347616e+06 |
| mean | 7.963902e+06 |
| std | 1.768098e+07 |
	
The volatility of 'talking about count' is examined. The result is shown in Figure 1.

<img src="Figures/Figure1.png" width="400">

## Facebook likes examination
The trend of Facebook likes gained over the years are examined. First, the absolute gain of Facebook likes for these food & beverage Facebook pages are computed and shown in Figure 2. 

 <img src="Figures/Figure2.png" width="400" >
	
Note: Dom=Dominos, PHut=Pizza Hut, PJ=PapaJohnUS, Chi=Chipotle, Stab=Starbucks, BK=Burger King

The absolute **likes** gain does not take into account the existing size of the page as well as the time taken to gain the likes. In order to get a more comparable data, the **likes values are normalised** and then **divided by the time frame** taken to gain those number of likes. The result is shown in Figure 3 for the top 10 food & beverage Facebook pages.  

<img src="Figures/Figure3.png" width="400" >

Note: Dom=Dominos, PHut=Pizza Hut, PJ=PapaJohnUS, Starb=Starbucks, Wen=Wendys, Chi=Chipotle, BK=Burger King

Analysing Figure 2 and 3, **ALL** Facebook pages in top 10 absolute likes gain also made to the top 10 normalised likes rate. 

The only different between these two figures is the **order** of the Facebook pages **Wendys, Chipotle and Strabucks**. In **Figure 2** (absolute likes gain) the order from 7-9 are as follows **Wendys, Chipotle then Strabucks**. While in **Figure 3** (normalised likes rate) the order from 7-9 are as follows **Strabucks, Wendys then Chipotle**.

Based on these observation, it can be concluded that **Strabucks** is likely to **overtake Wendys then Chipotle** in absolute gain chart(Figure 2) in the near future.

Next, the top 5 normalised likes rate Facebook pages are plotted against the time scale as shown in Figue 4. Note that, the latest date of the month and the total like at that time are used to develop the graph.

<img src="Figures/Figure4.png" width="500" >

Note: McDonalds and McDonaldsUS have almost identical growth and FB likes which made their graphs to overlap.

From Figure 4, it can be seen that the Facebook page **McDUS** (purple) and **McD** (red is overlapped) have the **steepest curve**, followed by **KFC** (light blue), **Dominos** (green), and then **PizzaHut** (yellow).

## Examination of relationship between Facebook likes and Facebook talking about count

Next the top 5 Facebook pages that showed the most likes gained over time are examined against the talking about count value. The aim here is to find whether there is a corelation between number or likes gained each month vs the talking about count. The number of likes gained each month determined by subtracting the newer month against the latest month likes count. While the average value of each month is used for talking about count value. Using these two values the corellation value is determined as shown in Table 4.

**Table 4:** Top 5 Facebook pages that showed the most likes gained over time correlation between likes gained each month and the talking about count

| Index | Facebook page name | Correlation | 
| --- | --- | --- |
| 1 | McDonalds | 0.536754 |
| 2 | McDonaldsUS | 0.107279 |
| 3 | KFC | -0.318145 |
| 4 | Dominos| 0.304336 |
| 5 | PizzaHut | 0.487411 |

McD (Figure 5) has the higest correlation between likes and talking about count among the top 5 normalised likes growth Facebook pages. While, KFC (Figure 6) has a negative relationship between likes and talking about count, a strange observation that requires further investigation.

<img src="Figures/Figure5.png" width="500" >

<img src="Figures/Figure6.png" width="500" >



