# Sudoku6x6Explainer

Sudoku6x6Explainer is my modifications to SudokuExplainer to solve 6x6 sudokus, with blocks of 2 rows x 3 columns.

There is some discussion about hard 6x6 sudokus here: http://forum.enjoysudoku.com/hardest-6x6-t35607.html

This version of Sudoku6x6Explainer was first released here: http://forum.enjoysudoku.com/post273912.html (2 January 2019).

I have since added a Dark theme, support for blocks of 3 rows x 2 columns, variants: Latin Square and Diagonals (X), an option for bigger cell size, and a 'Save as image...' option.

## Usage - GUI
```
java.exe -jar Sudoku6Explainer.jar
```
## Usage - serate
```
java.exe -Xrs -Xmx500m -cp Sudoku6Explainer.jar diuf.sudoku.test.serate --format="%g ED=%r/%p/%d" --input=puzzle(s).txt --output=output.txt [options]
```
## Usage - hints
```
java.exe -Xrs -Xmx500m -cp Sudoku6Explainer.jar diuf.sudoku.test.hints --input=puzzle(s).txt [options]

java.exe -Xrs -Xmx500m -cp Sudoku6Explainer.jar diuf.sudoku.test.hints --input=puzzle(s).txt 1>output.txt
java.exe -Xrs -Xmx500m -cp Sudoku6Explainer.jar diuf.sudoku.test.hints --input=puzzle(s).txt 1>output.txt 2>nul
```
STDOUT output (long hints) should (always) be redirected to a file.\
STDERR output (short hints) is for debug, it shows progress on screen, if not needed redirect this to a file or to nul.

## Usage - analyze (Tester)
```
java.exe -Xrs -Xmx500m -cp Sudoku6Explainer.jar diuf.sudoku.test.Tester puzzles.txt puzzles.log
```
## Options
None, one or a few of the following:
```
-2      for 2R x 3C (default)
-3      for 3R x 2C
-L      Latin Square
-X      Diagonals (X)
```
##### The options entered are not validated by the program, i.e. you can enter both -2 and -3, only one is used!
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

## Screenshots

![](/images/sudoku6.rc23.71.png)

2Rx3C, ED=7.1
```
....1..2...3.....4..56........34....  8 ED=7.1/1.2/1.2
```

![](/images/sudoku6.rc23.png)

2Rx3C
```
.....12....3..2.......45.16.........  8 ED=1.5/1.2/1.2
```
2Rx3C, Diagonals (X)
```
12.................34.....5.........  5 ED=1.5/1.2/1.2
```

![](/images/sudoku6.rc32.png)

3Rx2C
```
.......1..2.3..4..5..2......1......6  8 ED=1.5/1.2/1.2
```
3Rx2C, Diagonals (X)
```
.12...........3......4.............5  5 ED=1.5/1.2/1.2
```

![](/images/sudoku6.ls.png)

Latin Square
```
.1.2...2......3.4.......25.1......3.  9 ED=1.5/1.5/1.5
```
Latin Square, Diagonals (X)
```
....1........2.3........1.4.5.......  6 ED=1.5/1.5/1.5
```

