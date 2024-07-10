# Instructions
Please implement the provided interface `ExpenseCalculator` as per the problem statement below.
Do NOT change the interface.
Feel free to add classes as per your design.
Please use TDD.
Tests for everything you write is a MUST.
Please follow clean code principles.
## Getting Started
Create a Maven/Gradle project.
Create the classes as given in the following "Code Provided" section.
Implement the following interface in accordance with the problem statement.

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

### Problem Statement
Car rental application
A vehicle can be rented for a trip.
Vehicle can be an SUV, car, van, bus, etc.
The standard rate for a petrol vehicle for a standard trip is 0.20 EUR/Km.
Diesel vehicles cost 0.05 EUR less than the standard rate.
An additional 0.10 EUR/Km charge is applicable for AC vehicles.
Please note every vehicle has a maximum passenger capacity.
An additional charge of 0.05 EUR/Km/Person is imposed if the number of passengers exceeds the
max limit of a vehicle.
A 2% discount is applicable for buses on the standard rate.
The route of the trip always starts from Berlin.
All the distances to all destinations are specified in KM from Berlin.

### Example Values
Sample distance:
- Berlin: 0 KM
- Munich: 584 KM
- Hamburg: 289 KM
- Frankfurt: 545 KM
- Cologne: 576 KM


Do not use any property file to store the values mentioned above.
Think in terms of injectable interfaces to provide the information which will be developed later.
Please develop a default implementation for the same where data is hard coded.
The actual implementation of those may pull data from a database, file, or HTTP service.

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
The trip expense is 138.60 EUR.
