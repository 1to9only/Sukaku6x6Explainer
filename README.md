# Sudoku6x6Explainer

Sudoku6x6Explainer is my modifications to SudokuExplainer to solve 6x6 sudokus, with blocks of 2 rows x 3 columns.

There is some discussion about hard 6x6 sudokus here: http://forum.enjoysudoku.com/hardest-6x6-t35607.html

This version of Sudoku6x6Explainer was first released here: http://forum.enjoysudoku.com/post273912.html (2 January 2019).

## Usage - GUI

  java.exe -jar Sudoku6x6Explainer.jar

## Usage - serate

 java.exe -Xrs -Xmx500m -cp Sudoku6x6Explainer.jar diuf.sudoku.test.serate --format="%g ED=%r/%p/%d" --input=puzzles.txt --output=puzzles.rated.txt

## Usage - hints

  java.exe -Xrs -Xmx500m -cp Sudoku6x6Explainer.jar diuf.sudoku.test.hints --input=puzzle.txt

