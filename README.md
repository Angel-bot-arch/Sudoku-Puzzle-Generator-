# Sudoku-Puzzle-Generator
Made by Angel Wu
------
Description:
A unique Sudoku puzzle will be generated every time it is run. 

How to run: 
Copy and paste the code into a Java file (make sure the file is named SudokuPuzzleGenerator) and run the code. For example, using java sandbox https://codehs.com/explore/sandbox/java , create a new sandbox program: java(main), copy and paste the code from SudokuPuzzleGenerator_Code into the main file, change the main file name to SudokuPuzzleGenerator, and hit run.

How it works:
This code has 4 different methods with 4 different purposes:
- The fillBoard(int row, int col) method takes in two parameters, row and col, and it fills the board by picking a number, at random, checking that the number is valid, respective to its position on the board, and taking two routes: if valid it simply adds the number to the board, if invalid it generates a new number until the program gets a valid number. 
- The checker(int row, int col, int num) method is used in the fillBoard(int row, int col) method to ensure that it the number chosen is valid, in respect to it's position. So the checker method takes in the row, column, and number ints and makes sure that the number doesn't clash with any of the numbers in its row, column, or 3x3 square. 
- The shuffle(int a) method which is also used in the fillBoard(int row, int col) method to make the numbers unique. 
- The printBoard() method is to make the puzzle look nice and pretty by adding separators and borders( | or +-------+-------+-------+ ). It is also the method that prints out the board.
Using these methods, the main method creates a new SudokuPuzzleGenerator object and calls the fillBoard(int row, int col) method and has the program fill the board starting with the position (0,0). Afterwards, the program calls printBoard() which prints the board.

Files included: 
SudokuPuzzleGenerator.java
