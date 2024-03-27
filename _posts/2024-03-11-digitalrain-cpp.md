# Raining Matrix Blog

Hey there, I'm Connor, and today I'll be writing about a simple raining matrix effect I made in C++. My Matrix code is equipped with basic operations such as Constants, Seeding Random Number Generator, Boolean Array, Color Array, and Infinite loops. The program simulates a raining matrix effect by generating raindrops and characters falling down the console screen. It uses threading to run the matrix rain effect concurrently with the main program, enhancing the visual appeal of the simulation and it also switches from one function another using count variable.

## Header File
![image](https://github.com/connorngouana/rix/assets/115573354/a7058f92-5497-43c8-ad24-a9e684295067)

1. **Constructor:** Initializes the `RainingCode` class with the specified parameters, including the width and height of the console window and the sleep time between frames.
2. **startRainEffect():** This function initiates the rain effect, which simulates raindrops falling randomly on the screen.
3. **startMatrixRainEffect():** This function initiates the matrix rain effect, which creates a cascade of characters resembling the falling code from the movie "The Matrix."
4. **Drop Struct:** Defines a struct named `Drop` to represent individual raindrops. It contains members for the x and y coordinates of the raindrop, the distance it falls before resetting, and the length of its trail.
5. **setColor():** This is a helper function used internally to set the color of the console output.
6. **rainEffect():** This function displays the rain effect, showing characters randomly falling down the screen.
7. **Constants:** Various constants are defined, such as the character set (`CHARSET`), array of colors (`COLORS`), the number of colors available (`NUM_COLORS`), and the secondary bottom limit for raindrop fall distance (`SECONDARY_BOTTOM`).

### Cpp Code
Let's explain each function in the code separately:

![image](https://github.com/connorngouana/rix/assets/115573354/bb740661-2165-4c80-9759-be01996ad611)
### 1. startMatrixRainEffect() Function:
**Purpose:**
This function initiates the matrix rain effect, simulating raindrops falling down the screen in a manner reminiscent of the movie "The Matrix."

**Steps:**
**Initialization:**
- Initialize the random number generator using `srand(time(nullptr))`.
- Create a vector to store raindrop objects.
- Initialize variables for color index, raindrop count, and loop iteration.
**Raindrop Generation and Rendering:**
- Generate raindrop objects: If the number of raindrops is less than the screen width and a random condition is met, add a new raindrop to the vector.
- Clear the console screen (`"\033[2J\033[H"`) and set the color for the raindrops.
- Iterate through each raindrop:
  - Update the position of each raindrop.
  - If a raindrop reaches its fall distance, reset its position and characteristics.
  - Print characters representing raindrops at their positions on the console.
- Reset the color after rendering the raindrops.
**Animation Control:**
- Pause execution for a specified duration between frames using `std::this_thread::sleep_for()`.
- Repeat the process until the desired number of raindrop iterations is reached.

**Conclusion:**
After the animation completes, clear the screen and set a flag (`matrixRainFinished_`) to indicate that the matrix rain effect has finished.

![image](https://github.com/connorngouana/rix/assets/115573354/6689a3c0-0099-41d0-b9e0-1577e06a3a2b)



### 2. rainEffect() Function:

![image](https://github.com/connorngouana/rix/assets/115573354/24197bac-e856-4c2f-a8b9-30c4260cf337)


**Purpose:**
This function generates a simplified rain effect without color manipulation, resembling a basic rain animation.

**Steps:**
**Wait for Completion:**
Ensure the matrix rain effect has finished before starting the rain effect.
**Initialization:**
- Initialize the random number generator.
- Define the number of random flips per line.
**Raindrop Rendering:**
- For each line:
  - Randomly decide whether to display a raindrop character or empty space.
  - Print raindrop characters or spaces based on the decision.
  - Toggle switches randomly for the next line.
**Animation Control:**
- Pause execution for a specified duration between frames using `std::this_thread::sleep_for()`.
  
![image](https://github.com/connorngouana/rix/assets/115573354/0f7ef2a4-596b-44a3-857b-4e6daabbd360)



### Additional Information

- **Constants:** I define constants such as `WIDTH`, `HEIGHT`, `CHARSET`, `SLEEP_TIME`, `SECONDARY_BOTTOM`, and `COLORS` to control various aspects of the raining matrix effect.
- **Struct Definition:** I use a struct named `Drop` to represent individual raindrops. It contains members for position, fall distance, and length.

## Main File

![image](https://github.com/connorngouana/rix/assets/115573354/6c29bce5-2ceb-415e-a62e-7d182107b125)

In the main file, this program sets up a raining matrix effect simulation by creating a RainingCode object, starting the matrix rain effect in a separate thread, waiting for it to finish, and then initiating another rain effect.



## Conclusion

In conclusion, I've demonstrated how to create a raining matrix effect using Modern C++. By combining basic programming concepts with creativity, I've successfully crafted a visually captivating simulation.
