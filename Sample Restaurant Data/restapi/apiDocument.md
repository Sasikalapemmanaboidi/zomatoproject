// page 1
# List of City
>> https://zomatoajulypi.herokuapp.com/location
>> http://localhost:9700/location

# List of Restaurants
>> https://zomatoajulypi.herokuapp.com/restaurants
>> http://localhost:9700/restaurants

# List of Restaurants wrt to City
>> https://zomatoajulypi.herokuapp.com/restaurant?stateId=1
>> http://localhost:9700/restaurants?state_id=4

# List of MealType
>> https://zomatoajulypi.herokuapp.com/quicksearch
>> http://localhost:9700/mealType

//Page2
# List of restaurants on basis of meal
>> https://zomatoajulypi.herokuapp.com/restaurant?mealtype_id=
>> http://localhost:9700/restaurants?meal_id=4

# Filter on basis of cuisine
>> https://zomatoajulypi.herokuapp.com/filter/4?cuisine=1
http://localhost:9700/filters/3?cuisineId=4
# Filter on basis of cost
>> https://zomatoajulypi.herokuapp.com/filter/1?hcost=1000&lcost=500
http://localhost:9700/filters/1?lcost=300&hcost=900
# Sort (low to High)
http://localhost:9700/filters/1?cuisineId=4&sort=-1

//page3
# Details of restaurants
>> http://zomatoajulypi.herokuapp.com/details/1
>> http://localhost:9700/details/618776b162a1816f885956bf

Menu on the basis of restaurants
>>  http://localhost:9700/menu?restId=8

//page4 
> Menu details of item selected
(POST)> localhost:9700/menuItem
(body)> [1,4,6]

> Place Order
(post) > localhost:9700/placeOrder
(body) > 
{
    "name":"Sudha",
    "email":"sudha@gmail.com",
    "address":"dno:4-348,ramalayam street, madhavapatnam",
    "phone":6301393002,
    "cost":999,
    "menuItem":[1,33,51],
    "status":"Pending"
}

//page5
> See all order place
>>> localhost:9700/viewOrder
> Get Order on basis of emailId
>>>>  localhost:9700/viewOrder?email=sudha@gmail.com

//update order
(put) localhost:9700/updateOrder/6256fbab844264c34cb6125b
(body) 
{
	"status":"In Transit",
    "bankName":"Axis Bank"
}

