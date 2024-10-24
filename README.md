# Programming_Paradigms_Project

## Team Members

<table>
  <tr>
    <th>Name</th>
    <th>PRN</th>
  </tr>
    <tr>
    <td>Aditi Bansal</td>
    <td>23070122013</td>
  </tr>
  <tr>
    <td>Abhirami Nair</td>
    <td>23070122012</td>
  </tr>
  <tr>
    <td>Anagha Nair</td>
    <td>23070122027</td>
  </tr>
    <tr>
    <td>Afifa Bintul Hasan</td>
    <td>23070122017</td>
  </tr>
</table>

# Clazire Hotel Booking System

This application is designed for managing room bookings at Clazire Hotel, utilizing object-oriented programming principles to enhance code organization and reusability.

## Features

- **Room Types**: Choose between Normal and Luxury Rooms with different pricing and offers.
- **Dynamic Pricing**: Room charges are calculated based on the number of days and members.
- **Add-On Services**: Guests can opt for additional services like laundry and pool access.
- **Discount Offers**: Discounts are automatically applied based on specific conditions (e.g., number of members, length of stay).
- **Detailed Billing**: A comprehensive bill is generated showing all charges, discounts, and taxes.
- **Error Handling**: All types of errors are handled throighout the code.

## Object-Oriented Programming Concepts

### Hierarchical Inheritance

The system employs hierarchical inheritance by having a base class `Room` from which two derived classes, `NormalRoom` and `LuxuryRoom`, inherit. This structure allows the following:

- **Room Class**: Encapsulates common attributes and methods for all room types.
- **NormalRoom Class**: Inherits from `Room` and implements specific functionalities, such as discounts for larger groups.
- **LuxuryRoom Class**: Also inherits from `Room`, offering different pricing strategies and discount policies.

This hierarchy helps in reducing code duplication and improving maintainability.

### Polymorphism

Polymorphism is implemented through the following methods:

- **Virtual Functions**: The `Room` class defines virtual functions like `calculateDiscount()` and `getRoomType()`, which are overridden in the derived classes. This allows the program to call the appropriate method based on the object type at runtime.
  
- **Dynamic Binding**: When a derived class object is referenced using a base class pointer, the correct overridden method is invoked, allowing for flexibility and extensibility in the code.

## Code Explanation

The application consists of the following components:

1. **Room Class**: This is the base class containing attributes for guest name, number of days, number of members, room charge, buffet charge, tax percentage, and add-on service flags. It includes methods for calculating discounts, selecting add-on services, and displaying the bill.

2. **NormalRoom Class**: Inherits from the `Room` class. It initializes room charges specific to normal rooms and defines discount policies for groups larger than three members.

3. **LuxuryRoom Class**: Also inherits from the `Room` class. This class specifies room charges for luxury rooms and offers discounts for stays longer than five days.

4. **Main Function**: The entry point of the application that manages user interactions, allowing guests to input their details and select room types, ultimately leading to bill generation.

---

Thank you for exploring the Clazire Hotel Booking System! This project showcases effective use of OOP principles to create a robust and user-friendly booking experience.
