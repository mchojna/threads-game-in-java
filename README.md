# Threads Game in Java

This project is a multithreaded game implemented in Java. It features a graphical user interface (GUI) built with `Swing` and demonstrates the use of threads, concurrency, and game mechanics.

## Features

- **Player and Enemy Interaction**: The player can move, shoot, and interact with enemies.
- **Multithreading**: Tasks such as enemy creation and movement are handled using Java's `ExecutorService` and `Future`.
- **Game Mechanics**:
  - Shooting mechanics with single and double shots.
  - Ammo reloading and level progression.
  - Enemy health and damage system.
- **Custom Graphics**: The game uses custom graphics for the player, enemies, bullets, and background.
- **Task Management**: A separate panel allows managing tasks (e.g., enemy creation) with options to cancel, check state, and view results.

## Controls

- **A/D**: Move the player left/right.
- **L**: Single shot.
- **K**: Double shot (requires level 5 and sufficient ammo).
- **J**: Single shot from the left gun (requires level 5).
- **R**: Reload ammo.
- **C**: Clear bullets and blood from the screen.

## Classes Overview

### Core Classes

- **`Main`**: Initializes the game and GUI components.
- **`Player`**: Represents the player character with attributes like points, level, ammo, and kills.
- **`Enemy`**: Represents enemies with health and damage mechanics.
- **`Bullet`**: Represents bullets shot by the player.
- **`Blood`**: Visual effect for defeated enemies.
- **`Background`**: Renders the game background.

### GUI Components

- **`GamePanel`**: Handles the game rendering and player controls.
- **`AppPanel`**: Manages tasks (e.g., enemy creation) and displays their states in a `JList`.

### Utility Classes

- **`Element`**: Represents a basic drawable element with position, size, and color.
- **`Actor`**: Abstract class for characters like `Player` and `Enemy`.
- **`Drawable`**: Interface for drawable objects.

## How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/threads-game-in-java.git
   cd threads-game-in-java
   ```

2. Compile the project:

    ```bash
    javac -d out src/*.java
    ```

3. Run the game:

    ```bash
    java -cp out zad1.Main
    ```

## Requirements

- Java 8 or higher.
- A font file named `04B_19__.TTF` in the root directory (used for custom text rendering).

## Project Structure

    ```bash
    src/
    ├── [Actor.java](http://_vscodecontentref_/1)
    ├── [AppPanel.java](http://_vscodecontentref_/2)
    ├── [Background.java](http://_vscodecontentref_/3)
    ├── [Blood.java](http://_vscodecontentref_/4)
    ├── [Bullet.java](http://_vscodecontentref_/5)
    ├── [Drawable.java](http://_vscodecontentref_/6)
    ├── [Element.java](http://_vscodecontentref_/7)
    ├── [Enemy.java](http://_vscodecontentref_/8)
    ├── [GamePanel.java](http://_vscodecontentref_/9)
    ├── [Info.java](http://_vscodecontentref_/10)
    ├── [Main.java](http://_vscodecontentref_/11)
    ├── [Player.java](http://_vscodecontentref_/12)
    [UTP_C11_zadanie.html](http://_vscodecontentref_/13)
    [README.md](http://_vscodecontentref_/14)
    ```

## Future Improvements

- Add more enemy types and behaviors.
- Implement additional player abilities.
- Enhance the graphical interface.
- Add sound effects and music.
