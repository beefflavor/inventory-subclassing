# Object-Oriented Programming

![screenshot](screenshot.jpg)

## Description

Use inheritance in your inventory project. To do so, create at least five different classes for product categories. Each one should set a different value for the "category" field.

## Requirements

* Use `String.format` or `System.out.printf` anywhere you are manually concatenating strings with `+`.
* Create at least five classes that extend your existing inventory item class, each one representing a product category.
* Each category class should have a constructor that sets the "category" field to the appropriate name.
* Create a static `createItem` method in your main class which returns an object using the correct category class (or throws and error for an invalid category name).
  * `static InventoryItem createItem(String name, int quantity, String category)`

## Example
Please note this is just an example you should be using `private` class attributes.

```java
// parent class

public class Item {
    String name;
    int quantity;
    double price;
    String category;
}

// subclasses

public class Shoe extends InventoryItem {
    public Shoe(String name, double price, int quantity) {
        this.name = name;
        this.quantity = quantity;
        this.price = price;
        this.category = "Shoe";
    }
}

public class Shirt extends InventoryItem {
    public Shirt(String name, double price, int quantity) {
        this.name = name;
        this.quantity = quantity;
        this.price = price;
        this.category = "Shirt";
    }
}
```
