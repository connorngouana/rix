---
layout: post
title: A Project in Modern C++
tags: cpp coding project
categories: demo
---

![image](https://github.com/connorngouana/rix/assets/115573354/69234e0e-4ac3-4067-8e1c-5938c49e1b95)

## Raining Matrix Code
Hi Im Connor and today ill be writing about a  simple raining matix written in C++. The Matrix code comes loaded with basic operations such as Constants, Seeding Random Number Generator, Boolean Array, Color Array and Infinte loops.

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

## Conclusion

In conclusion, this project demonstrates how to create a captivating raining matrix effect using Modern C++. By combining basic programming concepts with creativity, I've successfully brought a piece of cinematic magic to life in the console environment. 

You can add an image that has been uploaded to the repository in a /docs/assets/images folder.
