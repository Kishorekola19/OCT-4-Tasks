# Multi-Floor Parking Lot Management System (LLD)

A robust, object-oriented Low-Level Design (LLD) implementation of a Multi-Floor Parking Lot Management System in C# (.NET).

## 🚀 Key Features

- **Multi-Floor Support:** Configurable floors with dedicated slots for different vehicle types (Motorcycle, Car, Truck, EV, Bus).
- **Flexible Slot Allocation Strategies:** Supports Lowest Floor First, Nearest Slot First, and Optimal Allocation strategies.
- **Dynamic Fee Calculation:** Strategy pattern implementation for Flat Rate, Hourly Rate, and Dynamic Vehicle-Tier pricing.
- **Ticket Management:** Automated ticket generation with timestamps, barcode/ID verification, and checkout fee processing.
- **Occupancy & Analytics Reporting:** Real-time floor occupancy, vacant slot tracking, and revenue reporting.
- **Comprehensive Unit Tests:** Full test coverage using MSTest/NUnit for core business logic and edge cases.

## 🛠️ Architecture & Design Patterns

- **Strategy Pattern:** `ISlotAllocationStrategy`, `IFeeStrategy`
- **Factory Pattern:** `VehicleFactory`, `FeeStrategyFactory`
- **Clean Architecture:** Strict separation between Models, Enums, Exceptions, Services, and Strategies.

## 📁 Project Structure

```
Multifloor-Parking-Lot-System/
├── Enums/            # SlotStatus, TicketStatus, VehicleType
├── Exceptions/       # Domain-specific custom exceptions
├── Factories/        # Object creation factories
├── Models/           # ParkingLot, ParkingFloor, ParkingSlot, Ticket, Vehicle
├── Services/         # IParkingLotService, ParkingLotService
├── Strategies/       # Allocation & Fee calculation strategies
├── tests/            # Unit testing suite
├── Program.cs        # Entry point / Console demo
└── Parking Lot Management System.csproj
```
