# Lab-3: Maven Pizza Factory Pattern

## Overview
A Java application that implements the Factory Design Pattern to create different types of pizzas, now using Maven for build management. Demonstrates the Liskov Substitution Principle and includes comprehensive JUnit 4 testing.

## Project Structure
```
Lab-3/
├── pom.xml
├── src/
│   ├── main/
│   │   └── java/
│   │       └── pizza/
│   │           ├── Pizza.java
│   │           ├── CheesePizza.java
│   │           ├── GreekPizza.java
│   │           ├── PepperoniPizza.java
│   │           ├── GlutenFreePizza.java
│   │           ├── VeganPizza.java
│   │           ├── PizzaType.java
│   │           ├── TranslatePizzaType.java
│   │           ├── PizzaFactory.java
│   │           └── PizzaStore.java
│   └── test/
│       └── java/
│           └── pizza/
│               └── PizzaFactoryTest.java
└── README.md
```

## Build and Run

### Compile Project
```bash
mvn clean compile
```

### Run Unit Tests
```bash
mvn test
```

### Run Main Program
```bash
mvn exec:java
```

### Package JAR
```bash
mvn package
```

### Clean Build
```bash
mvn clean
```

## Dependencies
Maven automatically manages:
- JUnit 4.13.2 (for testing)
- Hamcrest Core (JUnit dependency)

## Key Design Patterns
- **Factory Pattern**: PizzaFactory creates pizza objects based on type
- **Liskov Substitution Principle**: All pizza implementations can be used interchangeably
- **Interface Implementation**: All pizzas implement the Pizza interface

## Pizza Types
- Cheese Pizza
- Greek Pizza  
- Pepperoni Pizza
- Gluten-Free Pizza
- Vegan Pizza

## Example Output
The program demonstrates:
1. Connecticut pizza store opening
2. Processing customer orders for different pizza types
3. Complete pizza preparation process (prepare, bake, cut, box)
4. Liskov Substitution Principle with mixed pizza types

## Maven Benefits Over Lab-2
- **Automatic dependency management**: No manual JAR downloads
- **Standardized project structure**: Follows Maven conventions
- **Simplified build process**: Single commands for compile, test, run
- **IDE integration**: Most IDEs automatically recognize Maven projects
- **Professional setup**: Industry-standard build tool

## Test Results
All 5 JUnit tests pass successfully:
- Factory creates correct pizza types
- Store can process orders
- Liskov Substitution Principle demonstration

## AI Usage
Code generation assisted by Claude.ai 