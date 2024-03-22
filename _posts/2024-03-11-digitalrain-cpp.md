
![image](https://github.com/connorngouana/rix/assets/115573354/69234e0e-4ac3-4067-8e1c-5938c49e1b95)

## Raining Matrix Code
Hi Im Connor and today ill be writing about a  simple raining matix written in C++. The Matrix code comes loaded with basic operations such as Constants, Seeding Random Number Generator, Boolean Array, Color Array and Infinte loops.

## Header File

The header file `RAININGCODE.H` serves as the interface for our raining matrix effect program. Let's break down its components:

- **`width`**: Defines the width of the console window, determining the number of characters displayed horizontally.
- **`flipsPerLine`**: Specifies the number of character flips per line, adding randomness to the falling characters.
- **`sleepTime`**: Controls the delay between each frame of the animation, influencing the speed of the raining effect.
  ![image](https://github.com/connorngouana/rix/assets/115573354/5ad16f28-3bd6-4439-8ee9-a3942d62c7fa)


### Character Set

The `charSet` constant is a string that contains the characters used in the raining matrix effect. These characters are randomly chosen and displayed as falling raindrops in the console.
![image](https://github.com/connorngouana/rix/assets/115573354/ea97cb4e-f6d0-4372-bc3d-0c3b062693a5)


### Function Declaration

- **`rainEffect()`**: This function is declared without a return type or parameters. It is responsible for generating the raining matrix effect when invoked. The implementation of this function is defined in the corresponding source file.

### The Cpp File

I begin by including the necessary header files such as `"RAININGCODE.H"`, `<iostream>`, `<thread>`, `<cstdlib>`, `<ctime>`, and `<chrono>`. These headers provide functionalities for console I/O, multithreading, and random number generation, essential for my project.

### Creating the Matrix Effect

The core of my program lies within the `rainEffect()` function. Here's how it works:

1. **Color Manipulation**: I utilize ANSI escape codes to set different colors for the console output, enhancing the visual appeal of the matrix effect.
![image](https://github.com/connorngouana/rix/assets/115573354/9685764f-cd98-41d6-8f32-01fe6699e661)

2. **Random Character Generation**: Random characters from a predefined set are printed to the console, simulating the falling matrix code. I alternate between printing characters and spaces to create a realistic animation.
3. ![image](https://github.com/connorngouana/rix/assets/115573354/5298160c-d02f-4c30-8933-fd4fadc26f0e)

3. **Character Flipping**: To add variation to the falling characters, I randomly flip certain characters on each line, mimicking the randomness of raindrops.
 ![image](https://github.com/connorngouana/rix/assets/115573354/8c2440be-e301-4fc6-b373-f0b112ca1947)

 **Animation Control**: I introduce a delay between each frame using `std::this_thread::sleep_for()`, allowing me to control the speed of the animation. This creates a smooth and visually pleasing effect.
 ![image](https://github.com/connorngouana/rix/assets/115573354/c53861b7-9b11-4225-9b97-5c7a4305b9f9)

### Main File
The main file is just running the function that was previously mentioned in the Header part of the blog

## Conclusion

In conclusion, this project demonstrates how to create a  raining matrix effect using Modern C++. By combining basic programming concepts with creativity, I've successfully craeted a Raining Matrix. 

Sorry its late someone decided it was funny to tell me it was due on sunday and i believed and did check also changed my code didnt feel like tree code was good enough
