# vis.gchart

Chart library for [Zeppelin](http://zeppelin-project.org) based on [Google Chart](https://developers.google.com/chart/). This is meta file for online archive. 

Project source code and homepage are at [https://github.com/NFLabs/zeppelin-gchart](https://github.com/NFLabs/zeppelin-gchart)


## How to use

### Input data

* First Column - X axis data
* Second Column - Y axis data
* Third Column - Optional data

### Parameters

**type** - Set chart type selected by default. one of 'table' (default), 'pie', 'line', 'bar', 'area', 'bubble', 'column', 'guage', 'geo', 'map', 'scatter'. 

**height** - height of the chart in number. default 400.
   


## Example

Displaying 10 rows in table

    select * from bank limit 10 | vis.gchart;

Displaying line chart 

    select age, count(*) from bank group by age order by age | vis.gchart(type=line);


Displaying pie chart with height 200px 

    select job, count(*) from bank group by job | vis.gchart(type=pie,height=200);
