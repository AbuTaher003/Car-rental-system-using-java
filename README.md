# Car Rental System

This is a simple Java-based Car Rental System that allows users to rent and return cars interactively. The system provides features for managing cars, customers, and rental transactions, including support for electric cars.

## Features

- **Car Management:** Add and manage cars, including electric cars.
- **Customer Management:** Register new customers automatically during rentals.
- **Interactive Menu:** Allows users to rent, return, or exit the system easily.
- **Rental Transactions:** Calculate rental cost based on the number of days.
- **Electric Car Support:** Includes additional details like battery capacity.

## Classes and Structure

### 1. **Car Class**
- Represents a car with attributes such as `carId`, `brand`, `model`, `basePricePerDay`, and availability.
- Includes methods to calculate rental cost and manage availability.

### 2. **ElectricCar Class**
- Extends the `Car` class.
- Adds a unique property `batteryCapacity`.

### 3. **Customer Class**
- Represents a customer with attributes such as `customerId` and `name`.

### 4. **Rental Class**
- Represents a rental transaction, linking a car, a customer, and the rental duration.

### 5. **CarRentalSystem Class**
- Manages the cars, customers, and rentals.
- Provides the interactive menu for renting and returning cars.

### 6. **Main Class**
- Entry point for the application.
- Initializes the car rental system with sample cars and starts the menu.

## How to Run

1. Clone this repository:
   ```bash
   git clone <repository-url>
   ```
2. Navigate to the project directory:
   ```bash
   cd car-rental-system
   ```
3. Compile the Java files:
   ```bash
   javac Main.java
   ```
4. Run the program:
   ```bash
   java Main
   ```

## Sample Output

### Main Menu
```
=o==o= Rent your Dream Car =o==o=
1. Rent a Car
2. Return a Car
3. Exit
Enter your choice:
```

### Renting a Car
```
== Rent a Car ==

Enter your name: Taher

Available Cars:
C001 - Toyota Camry
C002 - Honda Accord
E001 - Tesla Model S

Enter the car ID you want to rent: E001
Enter the number of days for rental: 3

== Rental Information ==

Customer ID: CUS1
Customer Name: Taher
Car: Tesla Model S
Battery Capacity: 75 kWh
Rental Days: 3
Total Price: $300.00

Confirm rental (Y/N): Y

Car rented successfully.
```

### Returning a Car
```
== Return a Car ==

Enter the car ID you want to return: E001
Car returned successfully by Taher.
```

## Future Enhancements
- Add persistence to save rental records.
- Add user authentication for better security.
- Include more car attributes like mileage and fuel type.

## License
This project is open-source and available under the [MIT License](LICENSE).

---

Thank you for using the Car Rental System! Feel free to contribute or report any issues.

