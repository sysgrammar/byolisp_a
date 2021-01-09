# BYOLISP_A

## Project Info

**This project is a work in progress LISP**
This lisp is not meant for programming purposes but rather is a fun project of mine. I decided to write this as I wanted to learn C and do a fun project as well,

My source of learning is [BuildYourOwnLISP by Daniel Holden](https://buildyourownlisp.com/)

The book used in this project is written by [Daniel Holden](https://github.com/orangeduck), this book has been very insightful and fun to read and I am enjoying reading it.

I have also provided compiled binaries for windows and linux as well So that you can try what I have currently done
**[Download](https://github.com/sysgrammar/byolisp_a/releases)**

> Note: I will fully release when I finish reading the book

## Changelog (Begun since version early-0.4)
**Version `early-0.4`**
- Added error handling to the LISP
- Added two new opeartors: `min` and `max`
- Improved code readability
- Some cleanup and minor changes

**Version `early-00.5`**
- Added support for decimal input
- Added decimal calculations
- Added Symbolic Expressions like in a Typical Lisp
- Refactored Code

### Current Progress

- Able to get mathematical input in polish notation
- Returns syntax, mathematical errors i.e Too large numbers, division by zero etc
- Can perform the following mathematical opeartions
- Addition
- Subtraction
- Multiplication
- Division & remainder(modulus)
- Power
- Min/Max

### Syntax

**Addition**

To `add` two numbers
```byolisp_a> + 5 6```

To add more than two numbers
```byolisp_a> + 5 6 7 32 543```

**Subtraction**

To `sub` two numbers
```byolisp_a> - 5 6```

To sub more than two numbers
```byolisp_a> - 543 32 7 5```

**Multiplication**

To `mul` two numbers
```byolisp_a> * 5 6```

To mul more than two numbers
```byolisp_a> * 5 6 7 32 543```

**Division(Quotient)**

To `div` two numbers
```byolisp_a> / 30 5```

**Remainder**

To find the `rem` of two numbers
```byolisp_a> % 30 5```

**Power**

To find the `pow` of two numbers(Input base first and then the power to the base should be raised):
```byolisp_a> ^ 5 6```

**Minimum**
To return the `min` of two or more numbers entered:
```byolisp_a> min 4 39```

**Maximum**
To return the `max` of two or more numbers entered:
```byolisp_a> max 4 39```


## Compile Instructions

**Pre-requisites**
> must have any C compiler e.g GNU/GCC, Clang

**Compilation**

Place main.c mpc.c mpc.h in a single folder 

or

```git clone https://github.com/sysgrammar/byolisp_a.git```

```cd byolisp_a```
    
**Windows**

```gcc -std=c99 -Wall main.c mpc.c -lm -o byolisp_a```

**GNU/Linux**

```gcc -std=c99 -Wall main.c mpc.c -ledit -lm -o byolisp_a```

**NOTE(Linux users only)**

Editline could be missing from your distro and it may not compile, therefore you need to do this

>This command is for apt package manager 

```sudo apt-get install liibedit-dev```

Please note that arch users will have to modify the `main.c` file as history.c and readline.c have their names changed and are in separate locations.


### Goals

- Learn C
- Learning how a language is made
- Learning to write good code
- Complete this project.