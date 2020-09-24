<div align="center">

## Calculate fuel efficiency


</div>

### Description

Program calculates the fule effiency of the car on the trip in miles/gallon and the cost for gasoline at the end of the trip. It teaches begginer programmers functions and calculations.
 
### More Info
 
number of miles travel. the number of gallons purchased. and the price per gallon.

The fuel efficiency, miles per number of gallons, Gallons used on the trip, and The cost of the trip


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Wilton Marranzini](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/wilton-marranzini.md)
**Level**          |Beginner
**User Rating**    |5.0 (10 globes from 2 users)
**Compatibility**  |C\+\+ \(general\)
**Category**       |[Math](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/math__3-12.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/wilton-marranzini-calculate-fuel-efficiency__3-339/archive/master.zip)





### Source Code

```
/*
Author: Wilton Marranzini
Objective: Program calculates the fule effiency of the car on the trip in
miles/gallon and the cost for gasoline at the end of the trip.
*/
#include <iostream.h>           //including lib.
#include <math.h>             //including lib.
#include <cstring.h>           //including lib.
                     //Prototypes functions
void description();            //Description cout fuction.
float full_efficiency(int miles, int gallons);//efficiency function.
float cost(float price, int gallons);   //Cost function.
int main()                //Main Function
{ string gas_station;          //String for gas station name.
  int num_miles;             // Variable for number of miles
  int num_gallons;            //Variable for number of gallons.
  float price_per_gallons;        //Variable for price per gallons.
  float efficiency;           //variable for efficiency.
  float cos;               //variable for cost
  int a;                 //keeps screen function
  description();             //Discription function
  cout<< "Enter gas station name\n";
  getline(cin, gas_station);       //Getting gas station title
  cout<< "Name of gas station Is " << gas_station <<".\n";
  cout<<endl;
  cout<< "Enter the numbers of miles travel.\n";
  cin>>num_miles;//storing numbers of miles
  cout<< "Enter the number of gallons of gasoline purchased.\n";
  cin>>num_gallons;//storing number of gallons
  cout<< "Enter the Price per gallons.\n";
  cin>>price_per_gallons;        //storing price per gallons
  efficiency = full_efficiency(num_miles,num_gallons);//calling function.
  cos =cost(price_per_gallons,num_gallons);//calling function.
  cout<<"The efficiency is "<<efficiency<<" for "
    <<num_miles<<" miles per number of "<<num_gallons<<" gallons\n";
  cout<<"Gallons used on the trip is "<<num_gallons<<" The cost of the trip "
    <<"is "<<"$"<< cos <<endl;
  cin>>a;               //keeps screen open
  return 0;              //returning value
}
void description()
{
	cout<< "Program calculates the fule effiency of the car on the trip\n"
  	 << "in miles/gallon and the cost for gasoline at the end of the\n"
    << "trip.\n";
}
float full_efficiency(int miles, int gallons)
{
	float efficien;           //efficiency variable
	efficien = miles/gallons;
	return (efficien);          //returning value
}
float cost(float price, int gallons)
{
	float charge;            //charge variable
  charge = price*gallons;
  return (charge);           //returning value
}
```

