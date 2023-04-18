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
data_list = data.to_list()
print(data_list)

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

 
