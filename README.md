# Explore-Weather-Trends
First, I used sql to Extract the data, I chose Riyadh city where I live. I preferred to extract Riyadh city and the global together in one table so, my sql query was (
select city_data.country,city_data.city,city_data.year,city_data.avg_temp as
city_avg_temp,global_data.avg_temp as global_avg_temp
from city_list
join city_data
On city_list.city=city_data.city
join global_data
on global_data.year=city_data.year
where cit
y_list.city='Riyadh'; )
#opening up the CSV file
then, I used Excel to manipulate data and prepare my data for visualization.
I calculated the moving average for the 7 years, by inserting a new column E (Riyadh moving avg temperature) and wrote the function (=AVERAGE(D2:D8)) in E8 cell. Then I copied the function down.
#Creating a line chart
in order to smooth out the lines, making trends more observable, I decided to plot the moving average. Because we want to show trends over a period, line chart was the appropriate chart. And I used legend to differentiate both lines. Also, I wrote the chart title and axis labels.
#Making observations
Obviously, there is a big difference in temperatures. And the difference has been consistent over time. Riyadh is hotter on average compared with the global average temperature over years. The correlation coefficient between Riyadh and Global is 0.80, which leads to a positive and a strong relationship. Also, Riyadh and Global are getting hotter more and more, which means the world is getting hotter by years. And this has been consistence over years.
