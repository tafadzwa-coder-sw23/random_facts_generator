# random_facts_generator
# Random Fact Generator

This Python script generates random facts using the `randfacts` library.

## Features

* **Random Fact Generation:** The script uses the `randfacts` library to fetch and display a random fact each time you press Enter.
* **Simple Interface:** The script has a very simple command-line interface.

## How to Use

1.  **Install Python:** Make sure you have Python installed on your system.
2.  **Install the `randfacts` library:** Open a terminal or command prompt and install the library using pip:

    ```bash
    pip install randfacts
    ```

3.  **Run the script:** Save the Python code (e.g., as `random_facts.py`) and run it from your terminal:

    ```bash
    python random_facts.py
    ```

4.  **Get Random Facts:**
    * The script will print "Random Facts" to the console.
    * It will then prompt you with "Press Enter for Fact".
    * Press the Enter key.
    * The script will fetch a random fact and display it.
    * The script will continue to prompt you to press Enter for another fact until you interrupt the program (e.g., by pressing Ctrl+C).

## Code Description

The code does the following:

1.  **Imports:**
    * `os`:  While not directly used in the fact generation, it's often included in Python scripts for potential operating system interactions (which could be added later, such as clearing the screen).
    * `randfacts as rf`: Imports the `randfacts` library and assigns it the alias `rf` for brevity.

2.  **Prints a title:**
    * Prints "Random Facts" to the console.

3.  **Enters a loop:**
    * The `while x == ""` loop continues indefinitely until the user interrupts the program.
    * Inside the loop:
        * Prompts the user to "Press Enter for Fact".
        * Takes user input using `input()`.  The input is assigned to the variable `x`.  Because the loop condition is `x == ""`, the loop continues as long as the user only presses Enter (resulting in an empty string).
        * Fetches a random fact using `rf.get_fact()`.
        * Prints the random fact to the console.
