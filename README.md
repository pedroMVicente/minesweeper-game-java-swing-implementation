# Minesweeper Game - Java Swing Implementation

A fully-featured Minesweeper game built with Java Swing, featuring a custom UI, multiple difficulty levels, and classic minesweeper gameplay. This project demonstrates object-oriented design principles, event-driven programming, and GUI development in Java.

## 🎮 Game Overview

This is a complete implementation of the classic Minesweeper puzzle game where players must uncover all safe cells on a grid while avoiding hidden mines. The game features an intuitive graphical interface with three difficulty levels and real-time mine counting.

## Key Features

- **Three Difficulty Levels**:
  - 🟢 **Easy**: 8x8 grid with 20 mines
  - 🟡 **Medium**: 15x15 grid with 60 mines
  - 🔴 **Hard**: 20x20 grid with 120 mines

- **Intuitive GUI**: Custom-designed interface with Java Swing components
- **Mine Counter**: Digital-style display showing remaining mines
- **Game Status Display**: Real-time feedback on game state (Win/Loss/In Progress)
- **Restart Functionality**: Quick restart button to replay current difficulty
- **Custom Icons**: Visual indicators for mines, flags, and game elements
- **Responsive Design**: Clean, organized layout with custom fonts and colors

## 🎯 Game Rules

1. Click on cells to reveal them
2. Numbers indicate how many mines are adjacent to that cell
3. Use logic to deduce where mines are located
4. Avoid clicking on mines to win
5. Uncover all non-mine cells to complete the game

## 🛠️ Technologies Used

- **Java SE** - Core programming language
- **Java Swing** - GUI framework
- **AWT** - Graphics and event handling
- **Object-Oriented Programming** - Design patterns and architecture

## 📦 Installation & Setup

### Prerequisites
- Java Development Kit (JDK) 8 or higher
- Java IDE (Eclipse, IntelliJ IDEA, or NetBeans) - Optional

### Running the Game

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/minesweeper-java.git
cd minesweeper-java
```

2. **Compile the source code**
```bash
javac -d bin src/core/*.java src/visual/*.java
```

3. **Run the application**
```bash
java -cp bin visual.MainWindow
```

### Running from IDE
1. Import the project into your Java IDE
2. Ensure all resource files (images, fonts) are in the correct directories
3. Run `MainWindow.java` as the main class

## 🎨 UI Components

### Main Window Layout
- **North Panel**: Game title, mine counter, status display, and restart button
- **Center Panel**: Interactive game grid with clickable cells
- **West Panel**: Difficulty selection buttons (Easy, Medium, Hard)

### Color Scheme
- **Background**: Dark Gray (#3C3C3C)
- **Accent**: Orange (#FFA500)
- **Mine Counter**: Red Digital Display (#BF0802)
- **Borders**: Black with beveled effects

### Custom Features
- Digital 7-segment font for mine counter
- Custom button styling with icons
- Beveled borders for 3D effect
- Icon-text combinations for visual clarity

## 🧩 Core Components

### Game Class (`core/Game.java`)
- Manages game state (WON, LOST, NOT_FINISHED)
- Handles difficulty settings
- Processes player moves
- Checks win/loss conditions

**Constants:**
- `MINE = -1`: Represents a mine cell
- `LOST = 0`: Game lost state
- `WON = 1`: Game won state
- `NOT_FINISHED = 2`: Game in progress

**Key Methods:**
- `play(int line, int column)`: Processes cell selection
- `getState()`: Returns current game state
- `getGrid()`: Returns grid representation
- `getMines()`: Returns number of mines

### MainWindow Class (`visual/MainWindow.java`)
- Creates and manages the main application window
- Handles user interface layout
- Manages difficulty button actions
- Updates visual elements during gameplay

**Key Features:**
- 1500x1000 window size
- Custom panels for organization
- Event-driven button handlers
- Dynamic grid regeneration on difficulty change

## 📊 Game Difficulty Specifications

| Difficulty | Grid Size | Total Cells | Mines | Mine Density |
|-----------|-----------|-------------|-------|--------------|
| Easy      | 8x8       | 64          | 20    | 31.25%       |
| Medium    | 15x15     | 225         | 60    | 26.67%       |
| Hard      | 20x20     | 400         | 120   | 30.00%       |

## 🎓 Learning Outcomes

This project demonstrates:

1. **Object-Oriented Design**
   - Separation of concerns (core logic vs. visual components)
   - Encapsulation of game state and grid logic
   - Inheritance and polymorphism

2. **GUI Development**
   - Java Swing component hierarchy
   - Event listeners and action handlers
   - Custom UI component creation
   - Layout managers (BorderLayout, GridLayout)

3. **Game Development Concepts**
   - Grid-based game logic
   - State management
   - User interaction handling
   - Resource loading and management

4. **Software Engineering Practices**
   - Code organization and modularity
   - Constants for magic numbers
   - Resource management
   - Error handling

## 🚀 Features Implementation

### Grid Generation
- Random mine placement algorithm
- Ensures even distribution of mines
- Calculates adjacent mine counts for each cell

### Cell Revealing Logic
- Recursive unveiling of empty cells
- Adjacent cell counting
- Mine detection and game-over handling

### UI Updates
- Real-time mine counter updates
- Dynamic grid rendering based on difficulty
- Visual feedback for game states
- Smooth panel transitions on restart



## 📚 Topics Covered

- Java Programming
- Object-Oriented Programming (OOP)
- Java Swing GUI Development
- Event-Driven Programming
- Game Development
- Data Structures (Grid/Matrix)
- Algorithms (Random Generation, Recursion)
- Resource Management
- Software Design Patterns
- User Interface Design


⭐ If you enjoyed this project, please consider giving it a star!

**Made with ☕ and Java**
