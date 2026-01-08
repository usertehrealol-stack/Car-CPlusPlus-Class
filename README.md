# Car-C++-Class
This is a lesson about making a car class that uses a constructor to ask the user what the model is and save it to the Car's license-plate variable.

See car.cpp for the full code but I will put it here as well.

This is just a fun project and relatively for people who are really new to C++!

See my other projects as well; I made a Python password thingy.

# THE CODE!!
``` c++
// For the lesson, we will create a simple class named Car
// This is basically for C++ beginners to understand how a class works!!

// ISSUE; License plate formatting is not yet considered so you can make a random string as one; like abcjdsjiijasauijsasiusauiasui with no restrictions, but we dont need to focus on that now
// ISSUE; No error handling for input, so if you put in weird stuff it might break, but we dont need to focus on that now either

#include <iostream> // i/o (input output, like what you would see in Python with print(text))
#include <string> // using string data type, like in C with #include <string.h>
using namespace std; // Generally discouraged in most projects, but this is so we can make writing code easier; we don't have to use std::stuff every time

/* Car def, fun time!*/

class Car {
    public: // stuff we can use once called
        string licenseplate; // for license plate we will use later on
        string modelstr; // for model string
        Car() { // constructor, occurs once called
            cout << "Enter your model: " << endl; // prompt, endl is the same as /n (newline)
            cin >> modelstr; // get the model
            cout << "Enter your license plate: " << endl; // prompt for getting the license plate
            cin >> licenseplate; // get the license plate
        }

        // That's it. We can use a method to get the info once called

        void printInfo() {
            cout << "Model: " << modelstr << endl; // prints the model
            cout << "License Plate: " << licenseplate << endl; // prints the license plate
            cout << "Vroom...." << endl; // just for fun :D
        }
};

int main() { 
    // Our lovely main
    Car test_car;
    test_car.printInfo(); // call the print info method
    return 0; // end of program
}
```

You should get output like;
Enter your model:
Honda
Enter your license plate:
XX1-0002
Model: Honda
License Plate: XX1-0002
Vroom....

Try putting in other things; have fun! 

That's it for this lesson!!!
