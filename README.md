# Cinema Management System

## Overview

This project is a Cinema Management System developed in Java, utilizing **five creational design patterns**. Each design pattern is applied to different parts of the system to demonstrate their usage in a practical scenario.

### Design Patterns Used:
1. **Singleton Pattern**: Manages system configuration and ensures a single instance of global settings like cinema name and operating hours.
2. **Factory Method Pattern**: Allows the creation of different types of movies (e.g., RegularMovie, IMAXMovie).
3. **Abstract Factory Pattern**: Generates user interface elements (e.g., buttons) for different themes (DarkTheme, LightTheme).
4. **Builder Pattern**: Constructs complex ticket bookings with customizable options.
5. **Prototype Pattern**: Enables cloning and modification of movie schedules.

### Project Structure

```plaintext
.
├── src
│   ├── CinemaConfig.java           # Singleton Pattern
│   ├── Movie.java                  # Movie Interface
│   ├── RegularMovie.java           # Regular Movie (Factory)
│   ├── IMAXMovie.java              # IMAX Movie (Factory)
│   ├── MovieFactory.java           # Abstract Movie Factory
│   ├── RegularMovieFactory.java    # Factory for Regular Movies
│   ├── IMAXMovieFactory.java       # Factory for IMAX Movies
│   ├── Button.java                 # UI Component Interface
│   ├── DarkThemeButton.java        # Dark Theme Button
│   ├── LightThemeButton.java       # Light Theme Button
│   ├── UIFactory.java              # Abstract UI Factory
│   ├── DarkThemeFactory.java       # Factory for Dark Theme UI Components
│   ├── LightThemeFactory.java      # Factory for Light Theme UI Components
│   ├── TicketBooking.java          # Builder for Ticket Booking
│   ├── MovieSchedule.java          # Movie Schedule Interface (Prototype)
│   ├── StandardSchedule.java       # Standard Schedule Prototype
│   └── CinemaManagementApp.java    # Main Application
├── README.md                       # Project Documentation
