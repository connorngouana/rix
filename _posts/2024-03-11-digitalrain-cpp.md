![image](https://github.com/connorngouana/rix/assets/115573354/69234e0e-4ac3-4067-8e1c-5938c49e1b95)

## Raining Matrix Code
Hey there, I'm Connor, and today I'll be writing about a simple raining matrix effect I crafted in C++. My Matrix code is equipped with basic operations such as Constants, Seeding Random Number Generator, Boolean Array, Color Array, and Infinite loops.

![image](https://github.com/connorngouana/rix/assets/115573354/a3844d83-ab71-4b35-aeaf-1843491da7e1)

## Header File

Let's dive into the `RAININGCODE.H` header file, which serves as the interface for my raining matrix effect program. Here's the breakdown:

- **`startMatrixRainEffect()`**: This function declaration serves as the entry point for our simulation. It initiates the raining matrix effect when invoked.

### Function Declaration

In the `RAININGCODE.H` header file, I declare the `startMatrixRainEffect()` function without a return type or parameters. This function kicks off the raining matrix effect when called upon.

### The C++ File

The heart of my program lies within the `startMatrixRainEffect()` function. Here's how I've set it up:

1. **Color Manipulation**: I've employed ANSI escape codes to set different colors for the console output, enhancing the visual appeal of the matrix effect.
![image](https://github.com/connorngouana/rix/assets/115573354/32d76312-a1dd-4981-8d21-64735b72755f)

2. **Raindrop Generation**: I generate raindrop objects with random positions, fall distances, and lengths, simulating the falling matrix code.

  ![image](https://github.com/connorngouana/rix/assets/115573354/5723cfdd-f00a-48fa-b978-2cd19f1e99ac)

3. **Character Rendering**: Next, I iterate through the raindrop objects and print characters representing raindrops on the console. These characters are randomly selected from the character set.

 ![image](https://github.com/connorngouana/rix/assets/115573354/844a4cff-2cac-4b3d-91ac-b3b0f07f88c1)


4. **Animation Control**: To maintain a smooth visual experience, I introduce a delay between each frame using `std::this_thread::sleep_for()`. This allows me to control the speed of the animation.
   
![image](https://github.com/connorngouana/rix/assets/115573354/844a4cff-2cac-4b3d-91ac-b3b0f07f88c1)

### Additional Information

- **Constants**: I define constants such as `WIDTH`, `HEIGHT`, `CHARSET`, `SLEEP_TIME`, `SECONDARY_BOTTOM`, and `COLORS` to control various aspects of the raining matrix effect.

- **Struct Definition**: I use a struct named `Drop` to represent individual raindrops. It contains members for position, fall distance, and length.

### Main File

In the main file, I simply call the `startMatrixRainEffect()` function declared in the header file to initiate the raining matrix effect simulation.
![image](https://github.com/connorngouana/rix/assets/115573354/26d5f17f-ad8b-4559-9a5f-9380d5fc45d7)


## Conclusion

In conclusion, I've demonstrated how to create a raining matrix effect using Modern C++. By combining basic programming concepts with creativity, I've successfully crafted a visually captivating simulation.
