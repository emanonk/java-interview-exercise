# Instructions
Please implement the provided interface `ExpenseCalculator` as per the problem statement below.

* Do NOT change the interface.
* Feel free to add classes as per your design.
* Please use TDD.
* Tests for everything you write is a MUST.
* Please follow clean code principles.

## Getting Started
* Create a Maven/Gradle project.
* Create the classes as given in the following "Code Provided" section.
* Implement the following interface in accordance with the problem statement.

```java
    public interface ExpenseCalculator {
    /**
    @param vehicleType The type of selected vehicle (Car/Bus/Van etc.)
    @param fuelType The type of selected fuel (Diesel/Petrol)
    @param destination The selected destination
    @param numberOfPeopleTravelling The number of people traveling
    @param isAirConditioningRequired The selected option of air conditioning
    @return BigDecimal The calculated expense
    */
    BigDecimal calculateExpense(VehicleType vehicleType, FuelType fuelType, String destination, Integer numberOfPeopleTravelling, Boolean isAirConditioningRequired);
    }
```

### Problem Statement
Car rental application</br>
A vehicle can be rented for a trip.</br>
Vehicle can be an SUV, car, van, bus, etc.</br>
The standard rate for a petrol vehicle for a standard trip is 0.20 EUR/Km.</br>
Diesel vehicles cost 0.05 EUR less than the standard rate.</br>
An additional 0.10 EUR/Km charge is applicable for AC vehicles.</br>
Please note every vehicle has a maximum passenger capacity.</br>
An additional charge of 0.05 EUR/Km/Person is imposed if the number of passengers exceeds the
max limit of a vehicle.</br>
A 2% discount is applicable for buses on the standard rate.</br>
The route of the trip always starts from Berlin.</br>
All the distances to all destinations are specified in KM from Berlin.</br>

### Example Values
Sample distance:
- Berlin: 0 KM
- Munich: 584 KM
- Hamburg: 289 KM
- Frankfurt: 545 KM
- Cologne: 576 KM


Do not use any property file to store the values mentioned above.</br>
Think in terms of injectable interfaces to provide the information which will be developed later.</br>
Please develop a default implementation for the same where data is hard coded.</br>
The actual implementation of those may pull data from a database, file, or HTTP service.</br>

### Example Trip:
#### Given that
- Vehicle Type: Car
- Fuel Type: Petrol
- Destination: Munich
- Number of People Travelling: 5
- Is Air Conditioning Required: true
- Max Passenger Capacity of Selected Vehicle: 5
#### When
A customer books a trip.
#### Then
The trip expense is 175.2 EUR.

## Exercise completion guide
Please clone the current repository and create a private repo under your account.
Then please add this emanonk as a collaborator to your project/repo.

## Deliverables
I know how difficult is to find time to complete this exercise, so to make your life easier, you will decide how much time you will spend on this exercise.
This is why its important to include a readme file in your repo, and explain which areas you want to focus. 
For example, you can provide 1 unit test as an example, and then you can write down the test cases you would like to cover without the implementation.
If you manage to implement 1 test, then I know you write the others.

### Extra tips
Think as you are the interviewer, what are the things that you wish to see from the candidate? 
- It is not important to see 20 unit test implementation, it is important though to see the way of thinking and the test cases.
- Focus only on what is requested in the exercise. If you want to demonstrate more than that, be careful and cover everything that comes with that.
- Read the instructions more that one times.
- Feel free to use chatgpt or copilot, but please mention it in the readme and explain how you used it.
