# C-Basics

## 1. Data Types

| Data Type | Description |
|-----------|-------------|
| `int` | Used to store whole numbers (integers), typically 4 bytes in size. |
| `float` | Used to store single-precision floating-point (decimal) numbers, typically 4 bytes. |
| `double` | Used to store double-precision floating-point numbers, offering more precision than `float`, typically 8 bytes. |
| `char` | Used to store a single character, typically 1 byte, represented internally as an ASCII value. |
| `bool` | Used to store a boolean value: `true` or `false` (requires `stdbool.h` in C). |
| `void` | Represents "no value" or "no type"; used for functions that don't return a value or for generic pointers. |

## 2. Format Specifiers

| Specifier | Meaning |
|-----------|---------|
| `%d` | Signed decimal integer |
| `%u` | Unsigned decimal integer |
| `%o` | Unsigned octal integer |
| `%x` | Unsigned hexadecimal integer (lowercase letters) |
| `%X` | Unsigned hexadecimal integer (uppercase letters) |
| `%f` | Floating-point number (decimal notation) |
| `%e` | Floating-point number (scientific/exponential notation) |
| `%c` | Single character |
| `%s` | String of characters |
| `%ld` | Signed long integer |

## 3. Input/Output Functions

- **`scanf()`** — Reads formatted input from the user (keyboard) and stores it into variables, using format specifiers to interpret the input type.
- **`printf()`** — Prints formatted output to the screen, using format specifiers to control how values are displayed.
- **`getchar()`** — Reads a single character from standard input (keyboard).
- **`putchar()`** — Writes a single character to standard output (screen).
- **`fgets()`** — Reads a line of text (including spaces) from input into a string, up to a specified length or until a newline.
- **`puts()`** — Writes a string to standard output and automatically appends a newline at the end.

## 4. Escape Sequences

| Escape Sequence | Meaning | Example |
|------------------|---------|---------|
| `\n` | New line | `printf("Hello\nWorld");` |
| `\t` | Horizontal tab | `printf("A\tB");` |
| `\\` | Backslash character | `printf("C:\\Users");` |
| `\"` | Double quote character | `printf("She said \"Hi\"");` |
| `\'` | Single quote character | `printf("It\'s fine");` |

## 5. Precision for Floating-Point Output

Precision for floating-point output is specified by placing a period (`.`) followed by a number between the `%` and the conversion character (like `f`). This number tells `printf()` how many digits to display after the decimal point.

For example:
- `printf("%.2f", 3.14159);` → outputs `3.14`
- `printf("%.4f", 3.14159);` → outputs `3.1416`

If no precision is specified, `%f` defaults to 6 digits after the decimal point.
