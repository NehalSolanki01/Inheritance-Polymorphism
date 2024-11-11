# INHERITANCE-POLYMORPHISM

# 1. Fibonacci Series Generator

A Python application that generates the Fibonacci series using both iterative and recursive methods. The application has a graphical user interface (GUI) built with Tkinter, allowing users to input the number of terms they want to generate, and it provides two options for series generation: Iterative and Recursive.

## Features

- **Iterative Fibonacci**: Uses an iterative approach to generate the Fibonacci series.
- **Recursive Fibonacci**: Uses recursion to generate the Fibonacci series.
- **GUI**: Provides a simple Tkinter-based GUI where users can input the number of terms and choose the method to generate the series.
- **Error Handling**: Handles invalid input, ensuring users can only enter positive integers.

## Requirements

- Python 3.x
- Tkinter (typically comes pre-installed with Python)

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/NehalSolanki01/Inheritance-Polymorphism.git
   ```

2. Navigate to the project folder:

   ```bash
   cd Inheritance-Polymorphism
   ```

3. Run the Python script:

   ```bash
   python fibonacci_gui.py
   ```

   (Note: If your system does not have Tkinter installed, you may need to install it separately. On most systems, Tkinter comes pre-installed with Python.)

## Code Explanation

### 1. `SeriesGenerator` (Base Class)
The `SeriesGenerator` class is an abstract base class that defines the method `generate_series(n)`. This method should be overridden in the subclasses to implement specific series generation logic.

### 2. `FibonacciIterative` (Iterative Method)
The `FibonacciIterative` class inherits from `SeriesGenerator` and implements the `generate_series(n)` method iteratively. It starts with `a=0` and `b=1`, and for each term, it appends `a` to the series and updates `a` and `b` accordingly.

### 3. `Fib_Recursive` (Recursive Method)
The `Fib_Recursive` class also inherits from `SeriesGenerator` and implements the `generate_series(n)` method recursively. A helper function `fib(num)` is used to calculate the nth Fibonacci number by recursively calling itself.

### 4. `Fib_GUI` (Graphical User Interface)
The `Fib_GUI` class creates a Tkinter window that allows the user to:
- Enter the number of terms to generate.
- Choose between the iterative or recursive method to generate the Fibonacci series.
- Display the generated Fibonacci series.

The `generate_series` method takes a `generator` instance as an argument (either `FibonacciIterative` or `Fib_Recursive`) and generates the series based on user input. It also handles invalid input by displaying an error message.

### 5. Running the Application
When the script is run, the `Fib_GUI` class initializes a Tkinter window where users can input the number of terms they wish to generate, and click the respective buttons to generate the Fibonacci series either iteratively or recursively.

### Example Usage
1. **Enter the number of terms** (e.g., 10).
2. **Click "Generate Iteratively"** or **"Generate Recursively"**.
3. The Fibonacci series will be displayed on the window.

## Screenshots

(Here you can include some screenshots of the app in action, if you wish!)

## Contributing

Feel free to fork the repository and submit pull requests. If you encounter any issues or have suggestions for improvements, please open an issue.

## License

This project is open-source and available under the MIT License.

