# Qalculate! GTK+ UI

<a href="https://github.com/Qalculate/qalculate-gtk/raw/master/data/qalculate-gtk-appdata-1.png"><img src="https://github.com/Qalculate/qalculate-gtk/raw/master/data/qalculate-gtk-appdata-1.png" width="446"></a>

Qalculate! is a multi-purpose cross-platform desktop calculator. It is simple to use but provides power and versatility normally reserved for complicated math packages, as well as useful tools for everyday needs (such as currency conversion and percent calculation). Features include a large library of customizable functions, unit calculations and conversion, symbolic calculations (including integrals and equations), arbitrary precision, uncertainty propagation, interval arithmetic, plotting, and a user-friendly interface (GTK+ and CLI).

## Installation
In a terminal window in the top source code directory run
* `./autogen.sh` *(not required if using a release source tarball, only if using the git version)*
* `./configure`
* `make`
* `make install`

If libqalculate has been installed in the default /usr/local path you it might be necessary to specify the pkgconfig path when running configure:
`PKG_CONFIG_PATH=/usr/local/lib/pkgconfig ./configure`

## Requirements
* GTK+ (>= 3.10)
* libqalculate 2.8.0

## Features
Features specific to qalculate-gtk:

* Graphical user interface implemented using GTK+-3
* Flexible expression entry and separate result display
* Displays whether result is precise or not
* Small and ... not so small mode
* Practical menus give fast access to all advanced features
* Calculation history
* Optional traditional calculator buttons
* Dialogs for management of and easy access to functions, variables and units (with quick conversion)
* User friendly dialogs for functions, with description and entries for arguments
* Create/edit functions, variables and units
* Easy editing of matrices and vectors
* Easy interface to gnuplot
* Separate window for fast conversion between number bases
* Periodic table
* Small separate utilities for base, currency and unit conversion
* Additional text based interface with full functionality
* and more...

Features from libqalculate:

* Calculation and parsing:
   * Basic operations and operators: + - * / ^ E () && || ! < > >= <= != ~ & | << >>
   * Fault-tolerant parsing of strings: log 5 / 2 .5 (3) + (2( 3 +5 = ln(5) / (2.5 * 3) + 2 * (3 + 5)
   * Expressions may contain any combination of numbers, functions, units, variables, vectors and matrices, and dates
   * Supports complex and infinite numbers
   * Propagation of uncertainty
   * Interval arithmetic (for determination of the number of significant digits or direct calculation with intervals of numbers)
   * Supports all number bases from 2 to 36, time format and roman numerals
   * Ability to disable functions, variables, units or unknown variables for less confusion: ex. when you do not want (a+b)^2 to mean (are+barn)^2 but ("a"+"b")^2
   * Controllable implicit multiplication
   * Matrices and vectors, and related operations (determinants etc.)
   * Verbose error messages
   * Arbitrary precision
   * Interval arithmetics
   * RPN mode
* Result display:
   * Supports all number bases from 2 to 36, plus sexagesimal numbers, time format and roman numerals
   * Many customization options: precision, max/min decimals, multiplication sign, etc.
   * Exact or approximate
   * Fractions: 4 / 6 * 2 = 1.333... = 4/3 = 1 + 1/3
* Symbolic calculation:
   * Ex. (x + y)^2 = x^2 + 2xy + y^2; 4 "apples" + 3 "oranges"
   * Factorization and simplification
   * Differentiation and integration
   * Can solve most equations and inequalities
   * Customizable assumptions give different results (ex. ln(2x) = ln(2) + ln(x) if x is assumed positive)
* Functions:
   * All the usual functions: sine, log, etc... : ln 5 = 1.609; sqrt(tan(20) - 5) = sqrt(-2.76283905578)
   * Lots of statistical, financial, geometrical, and more functions (approx. 200)
   * If..then..else function, optional arguments and more features for flexible function creation
   * Can easily be created, edit and saved to a standard XML file
* Units:
   * Supports all SI units and prefixes (including binary), as well as imperial and other unit systems
   * Automatic conversion: ft + yd + m = 2.2192 m
   * Implicit conversion: 5m/s to mi/h = 11.18 miles/hour
   * Smart conversion: can automatically convert 5 kg*m/s^2 to 5 newton
   * Currency conversion with retrieval of daily exchange rates
   * Different name forms: abbreviation, singular, plural (m, meter, meters)
   * Can easily be created, edit and saved to a standard XML file
* Variables and constants:
   * Basic constants: pi, e
   * Lots of physical constants and elements
   * CSV file import and export
   * Can easily be created, edit and saved to a standard XML file
   * Flexible, can contain simple numbers, units or whole expressions
   * Data sets with objects and associated properties in database-like structure
* Plotting:
   * Uses Gnuplot
   * Can plot functions or data (matrices and vectors)
   * Ability to save plot to PNG image, postscript, etc.
   * Several customization options
* and more...
