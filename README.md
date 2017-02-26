# lifeguide.food.crawlers
crawlers getting some food data for my personal use

Food data assumptions:
1. Assumption: Food knowledge is pretty much static, eg protein amount in specific product won't change

  => We are endeavor to make every product fully described with consistand, non duplicated information about every nutrient. We don't need to duplicate nutrient info in each recipie. We can make simple reference to every product and calculate nutrient value based on products

2. Data sources can vary between each other, are different in quality 
  - same product can have differnt details in two different sources     
  - same propduct can have mutual exclusive details 
  
  
  => we will have two databases 
     - raw data to collect nutrient value with data source
     - final data with single and final values
  => we need to have tools to map from raw data to final one
  => process of preparing products database is long and we will grow it over time. Meantime we can have final data comming from one source    to move one with next functionality 
  => we will keep reference do sources for each product 
  
  
3. Data will grow over time especially in area of diets and recipies
   => we need to web scrape same sources multiple time searching for new things
   => we can ommit already existing ones or calculate hash of it because they are not likely to change frequently
   
1# Downloads json data from specific url
2# Converts any data into common format
3# 
