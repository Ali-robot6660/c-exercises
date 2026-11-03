# C Exercises

My practice programs from learning the C language: basic input/output, loops, arrays, functions, pointers and structures.

## Structure

```
c-exercises/
├── basics/          # small standalone programs
└── book-exercises/  # exercises from a C textbook (page numbers are in the comments)
```

### basics/

| File | What it does |
|---|---|
| `input_output.c` | Reads your age and prints it back |
| `hours_to_minutes_seconds.c` | Converts hours and minutes into total minutes and seconds |
| `days_of_week.c` | Prints the day of the week for a number 1–7 (`switch`) |
| `factorial.c` | Multiplies the numbers 1 to 10 (10!) |
| `fibonacci.c` | Prints Fibonacci numbers using a function |
| `powers.c` | Square, cube, 4th and 5th power of a number |
| `multiplication_table.c` | Multiplication table for one number (`for`) |
| `multiplication_table_while.c` | Full multiplication table (`while`) |
| `multiplication_table_array.c` | Multiplication table stored in a 2D array |
| `rhombus.c` | Draws a rhombus of `*` of a given size |

### book-exercises/

Loops (`for1`, `for2`, `while1`, `while2`, `do_while`), `switch` (`switch_case`), a star pattern (`page53_star_pattern`),
and textbook exercises on arrays, pointers, functions and structures (`exercise_*.c`).
Some exercise files contain several solutions; the inactive ones are commented out.

## How to build and run

You need a C compiler, for example GCC (MinGW / MSYS2 on Windows).

```bash
gcc basics/rhombus.c -o rhombus
./rhombus
```

`powers.c` uses `math.h`; on Linux add `-lm`:

```bash
gcc basics/powers.c -o powers -lm
```

Some programs print Korean or Russian text. On Windows, switch the console to UTF-8 first: `chcp 65001`.

## Example

```
$ ./rhombus
Enter number for rhombus: 3
  *
 ***
*****
 ***
  *
```
