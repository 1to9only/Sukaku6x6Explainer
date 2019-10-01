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

# Sukaku6x6Explainer

Sukaku6x6Explainer is my modifications to Sudoku6x6Explainer to support 6x6 sukakus.

Sukaku6x6Explainer supports loading of single-line 6x6 sudokus (36 characters):
```
..3...4.....2..3.5.....1.6.5.45...1.
```

and single-line 6x6 sukakus (216 characters):
```
1....612..5...3...12.4.6.2.456.2...6...4..12..5.12..5612...6.23.56.23..6.2....1..4..1..4.6..3......4.6....5...3..6..345....456.2.4.6.2.4.61.....1.3........612........5..23......4......5..234...2.4...2...61......23..6
```

Usage is as for Sudoku6x6Explainer

