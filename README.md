# Geo-Economic-Clustering

Geo-economic Clustering

A company has decided to expand and open new markets, and the CEO has asked the Data Science team to
help define the strategy by classifying all countries in the world in different geo-economic groups.
The task at hand is to classify all countries in the world in 10 different groups according to the
distance between them and their GDP (Gross Domestic Product) per capita.
You will need to find information about each country’s GDP and GDP per capita, as well as their
physical coordinates on Earth (you can assume that each country is located at the latitude and
longitude of its capital city, their geographical center or any other representative point that you
consider adequate for the task) and create 10 groups of countries that are close together *and* have
similar GDP per capita.
The output would be a comma (or tab) separated value with as many lines as there are countries in the
world. The required columns are
1.
country name or code
2.
group label (from 0 to 9)
3.
group’s average GDP per capita
4.
country’s GDP per capita
5.
country’s total GDP
6.
cumulative GDP fraction (0 to 1) within the group (after ordering; see next paragraph)
The data should be ordered according to the following hierarchy:
1.
group’s average GDP per capita
2.
country’s total GDP
This means that the group with the highest average GDP per capita should be at the beginning (top) of
the data structure, and the group with the lowest GDP per capita at the end (bottom). Then, within
each group, the country with the highest total GDP should be at the beginning of the group and the
country with the lowest GDP at the end of the group.
The cumulative GDP fraction within each group should be calculated with this order in mind (highest
total GDP first)
