# Parking Lot Management Application

A simple parking lot management system built in Java. You can manage parking slots, park vehicles, and track occupancy - all from either a command line or web interface.

## What This Project Does

This is a parking lot management system that lets you:

- Set up a parking lot with different sized slots (Small, Large, Oversize)
- Park vehicles and automatically assign them to the right sized slot
- Remove vehicles when they leave
- See the current status of all parking slots

## How It Works

The app uses a simple strategy pattern to find the best parking spot for each vehicle. Small cars can fit in any slot, large cars need large or oversize slots, and oversize vehicles need oversize slots.

### Key Features

- **Flexible Setup**: Choose how many slots of each size you want
- **Smart Parking**: Automatically finds the right spot for each vehicle
- **Two Interfaces**: Use it from the command line or through a web browser
- **Real-time Status**: See which slots are occupied and which are free

## 🌐 Live Demo

**Try the web interface online!**

The application is deployed on Render and available at: [https://parkinglotmanagerweb.onrender.com](https://parkinglotmanagerweb.onrender.com)

## Getting Started

### Prerequisites

- Java 17 or higher
- Maven 3.6 or higher
- A web browser (for the web version)

### Running the CLI Version

1. Open terminal and go to the CLI folder:

   ```bash
   cd ParkingLotManager
   ```

2. Compile and run:

   ```bash
   mvn clean compile
   mvn exec:java -Dexec.mainClass="main"
   ```

3. Follow the prompts:
   - Enter how many total slots you want
   - Choose from the menu (Park, Remove, Status, Exit)

### Running the Web Version

1. Open terminal and go to the web folder:

   ```bash
   cd ParkingLotManagerWeb
   ```

2. Start the application:

   ```bash
   mvn spring-boot:run
   ```

3. Open your browser and go to: `http://localhost:8080`
   - First time, you'll set up your parking lot
   - Then you can start parking vehicles!

## Testing

To run the tests:

**CLI tests:**

```bash
cd ParkingLotManager
mvn test
```

**Web tests:**

```bash
cd ParkingLotManagerWeb
mvn test
```
