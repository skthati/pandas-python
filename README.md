<a name="readme-top"></a>


<div align="center">
<!-- Title: -->
<h1><a href="https://github.com/skthati/pandas-python/">Pandas</a> - Python </h1>
</div>

<!-- Table of contents -->
<hr>
<hr>
<ol>
    <li><a href="#pandas">Pandas</a></li>
    <li><a href="#bloopers">Bloopers</a></li>
</ol>
<hr>
<hr>




# Pandas
To get all data from CSV 

CSV is :
```
day	temp	condition
Monday	12	Sunny
Tuesday	14	Rain
Wednesday	15	Rain
Thursday	14	Cloudy
Friday	21	Sunny
Saturday	22	Sunny
Sunday	24	Sunny
```

 ```Python
 import pandas
 
data = pandas.read_csv("weather-data.csv")
print(data)

```

To get a column from csv

```Python
print(data["temp"])

```
### Series 
Is 1 dimentional data

### Dataset 
Is 2 dimentional data

To Check datatype of data
```Python
print(type(data["temp"]))

```

### Data_dict
To convert data to data dictionary

```Python
data_dict = data.to_dict()
print(data_dict)
```
### Data_list
To convert data to data list.

```Python
data_list = data["temp"].to_list()
print(data_list)

```
### Average
```Python
data["temp"].mean()
```

### Max

```Python
data["temp"].max()

```

## Data Rows
To get the entire row in pandas.

```Python
data[data.temp == "Monday"]
#OR
data[data["temp"] == "Monday"]
```

To print the row which has max temperature

```Python
print(data[data.temp == data.temp.max()])
```

To print the row specific series(column) data

```Python
x = data[data.day == "Monday"]
print(x.condition)

result is sunny.
```

## Data frames
To convert data to data frames.

```Python
data_dict = {
    "students" = ["Amy", "James", "John"],
    "age" = [23, 34, 45]
}

data = pandas.DataFrame(data_dict)
#print(data)
data.to_csv("new_file.csv")
```

## Squirrel color count. 
Import csv data and export to csv using dataframes

```Python
import pandas

data = pandas.read_csv("squirrel_data.csv")
gray_sqi_count = len(data[data["Primary Color"] == "Gray"])
red_sqi_count = len(data[data["Primary Color"] == "Red"])
black_sqi_count = len(data[data["Primary Color"] == "Black"])

data_dict = {
    "color": ["Gray", "Red", "Black"],
    "count": [gray_sqi_count, red_sqi_count, black_sqi_count]
}

#To save to another csv
df = pandas.DataFrame(data_dict)
df.to_csv("new_file.csv")
```



 ## Bloopers <a name="bloopers"></a>



<!-- 

Test1  
## Test <a name="test"></a>
Test Test

1. Code
    ```Python
    sc.onkey(key="Up", fun=up_move)
    sc.onkey(key="Right", fun=right_move)
    sc.onkey(key="Left", fun=left_move)
    sc.onkey(key="Down", fun=down_move)
    ```

2. Output

    ![Alt text](images/snake_working.gif)

<p align="right">(<a href="#readme-top">back to top</a>)</p>
<hr>  


-->

 
