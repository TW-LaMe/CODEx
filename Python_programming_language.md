


Python is a high-level, general-purpose programming language. Its design philosophy emphasizes code readability with the use of significant indentation.


Python is dynamically type-checked and garbage-collected. It supports multiple programming paradigms, including structured (particularly procedural), object-oriented and functional programming. It is often described as a "batteries included" language due to its comprehensive standard library.


Guido van Rossum began working on Python in the late 1980s as a successor to the ABC programming language and first released it in 1991 as Python 0.9.0. Python 2.0 was released in 2000. Python 3.0, released in 2008, was a major revision not completely backward-compatible with earlier versions. Python 2.7.18, released in 2020, was the last release of Python 2.


Python consistently ranks as one of the most popular programming languages, and has gained widespread use in the machine learning community.


## History

Python was conceived in the late 1980s by Guido van Rossum at Centrum Wiskunde & Informatica (CWI) in the Netherlands as a successor to the ABC programming language, which was inspired by SETL, capable of exception handling and interfacing with the Amoeba operating system. Its implementation began in December 1989. Van Rossum shouldered sole responsibility for the project, as the lead developer, until 12 July 2018, when he announced his "permanent vacation" from his responsibilities as Python's "benevolent dictator for life" (BDFL), a title the Python community bestowed upon him to reflect his long-term commitment as the project's chief decision-maker (he has since come out of retirement and is self-titled "BDFL-emeritus"). In January 2019, active Python core developers elected a five-member Steering Council to lead the project.


The name Python is said to come from the British comedy series Monty Python's Flying Circus.


Python 2.0 was released on 16 October 2000, with many major new features such as list comprehensions, cycle-detecting garbage collection, reference counting, and Unicode support. Python 2.7's end-of-life was initially set for 2015, then postponed to 2020 out of concern that a large body of existing code could not easily be forward-ported to Python 3. No further security patches or other improvements will be released for it. While Python 2.7 and older versions are officially unsupported, a different unofficial Python implementation, PyPy, continues to support Python 2, i.e. "2.7.18+" (plus 3.10), with the plus meaning (at least some) "backported security updates".


Python 3.0 was released on 3 December 2008, with some new semantics and changed syntax. At least every Python release since (now unsupported) 3.5 has added some syntax to the language, and a few later releases have dropped outdated modules, or changed semantics, at least in a minor way.


Since 7 October 2024, Python 3.13 is the latest stable release, and it and, for few more months, 3.12 are the only releases with active support including for bug fixes (as opposed to just for security) and Python 3.9, is the oldest supported version of Python (albeit in the 'security support' phase), due to Python 3.8 reaching end-of-life. Starting with 3.13, it and later versions have 2 years of full support (up from one and a half), followed by 3 years of security support (for same total support as before).


Security updates were expedited in 2021 (and again twice in 2022, and more fixed in 2023 and in September 2024 for Python 3.12.6 down to 3.8.20), since all Python versions were insecure (including 2.7) because of security issues leading to possible remote code execution and web-cache poisoning.


Python 3.10 added the | union type operator and the match and case keywords (for structural pattern matching statements). 3.11 expanded exception handling functionality. Python 3.12 added the new keyword type. Notable changes in 3.11 from 3.10 include increased program execution speed and improved error reporting. Python 3.11 claims to be between 10 and 60% faster than Python 3.10, and Python 3.12 adds another 5% on top of that. It also has improved error messages (again improved in 3.14), and many other changes.


Python 3.13 introduces more syntax for types, a new and improved interactive interpreter (REPL), featuring multi-line editing and color support; an incremental garbage collector (producing shorter pauses for collection in programs with a lot of objects, and addition to the improved speed in 3.11 and 3.12),  and an experimental just-in-time (JIT) compiler (such features, can/needs to be enabled specifically for the increase in speed), and an experimental free-threaded build mode, which disables the global interpreter lock (GIL), allowing threads to run more concurrently, that latter feature enabled with python3.13t or python3.13t.exe.


Python 3.13 introduces some change in behavior, i.e. new "well-defined semantics", fixing bugs (plus many removals of deprecated classes, functions and methods, and removed some of the C API and outdated modules): "The   implementation of locals() and frame.f_locals is slow, inconsistent and buggy  has many corner cases and oddities. Code that works around those may need to be changed. Code that uses locals() for simple templating, or print debugging, will continue to work correctly."


Some (more) standard library modules and many deprecated classes, functions and methods, will be removed in Python 3.15 or 3.16.


Python 3.11 adds Sigstore digital verification signatures for all CPython artifacts (in addition to PGP). Since use of PGP has been criticized by security practitioners,  Python is moving to Sigstore exclusively and dropping PGP from 3.14.


Python 3.14 is now in alpha 3; regarding possible change to annotations: "In Python 3.14, from __future__ import annotations will continue to work as it did before, converting annotations into strings."


PEP 711 proposes PyBI: a standard format for distributing Python Binaries.


Python 3.15 will "Make UTF-8 mode default", the mode exists in all current Python versions, but currently needs to be opted into. UTF-8 is already used, by default, on Windows (and elsewhere), for most things, but e.g. to open files it's not and enabling also makes code fully cross-platform, i.e. use UTF-8 for everything on all platforms.


## Design philosophy and features

Python is a multi-paradigm programming language. Object-oriented programming and structured programming are fully supported, and many of their features support functional programming and aspect-oriented programming (including metaprogramming and metaobjects). Many other paradigms are supported via extensions, including design by contract and logic programming. Python is often referred to as a 'glue language' because it can seamlessly integrate components written in other languages.


Python uses dynamic typing and a combination of reference counting and a cycle-detecting garbage collector for memory management. It uses dynamic name resolution (late binding), which binds method and variable names during program execution.


Its design offers some support for functional programming in the Lisp tradition. It has filter,mapandreduce functions; list comprehensions, dictionaries, sets, and generator expressions. The standard library has two modules (itertools and functools) that implement functional tools borrowed from Haskell and Standard ML.


Its core philosophy is summarized in the Zen of Python (PEP 20), which includes aphorisms such as:


However, Python features regularly violate these principles and have received criticism for adding unnecessary language bloat. Responses to these criticisms are that the Zen of Python is a guideline rather than a rule. The addition of some new features had been so controversial that Guido van Rossum resigned as Benevolent Dictator for Life following vitriol over the addition of the assignment expression operator in Python 3.8.


Nevertheless, rather than building all of its functionality into its core, Python was designed to be highly extensible via modules. This compact modularity has made it particularly popular as a means of adding programmable interfaces to existing applications. Van Rossum's vision of a small core language with a large standard library and easily extensible interpreter stemmed from his frustrations with ABC, which espoused the opposite approach.


Python claims to strive for a simpler, less-cluttered syntax and grammar while giving developers a choice in their coding methodology. In contrast to Perl's "there is more than one way to do it" motto, Python embraces a "there should be one—and preferably only one—obvious way to do it." philosophy. In practice, however, Python provides many ways to achieve the same task. There are, for example, at least three ways to format a string literal, with no certainty as to which one a programmer should use. Alex Martelli, a Fellow at the Python Software Foundation and Python book author, wrote: "To describe something as 'clever' is not considered a compliment in the Python culture."


Python's developers usually strive to avoid premature optimization and reject patches to non-critical parts of the CPython reference implementation that would offer marginal increases in speed at the cost of clarity. Execution speed can be improved by moving speed-critical functions to extension modules written in languages such as C, or by using a just-in-time compiler like PyPy. It is also possible to cross-compile to other languages, but it either doesn't provide the full speed-up that might be expected, since Python is a very dynamic language, or a restricted subset of Python is compiled, and possibly semantics are slightly changed.


Python's developers aim for it to be fun to use. This is reflected in its name—a tribute to the British comedy group Monty Python—and in occasionally playful approaches to tutorials and reference materials, such as the use of the terms "spam" and "eggs" (a reference to a Monty Python sketch) in examples, instead of the often-used "foo" and "bar". A common neologism in the Python community is pythonic, which has a wide range of meanings related to program style. "Pythonic" code may use Python idioms well, be natural or show fluency in the language, or conform with Python's minimalist philosophy and emphasis on readability. Code that is difficult to understand or reads like a rough transcription from another programming language is called unpythonic.


## Syntax and semantics

Python is meant to be an easily readable language. Its formatting is visually uncluttered and often uses English keywords where other languages use punctuation. Unlike many other languages, it does not use curly brackets to delimit blocks, and semicolons after statements are allowed but rarely used. It has fewer syntactic exceptions and special cases than C or Pascal.


### Indentation

Python uses whitespace indentation, rather than curly brackets or keywords, to delimit blocks. An increase in indentation comes after certain statements; a decrease in indentation signifies the end of the current block. Thus, the program's visual structure accurately represents its semantic structure. This feature is sometimes termed the off-side rule. Some other languages use indentation this way; but in most, indentation has no semantic meaning. The recommended indent size is four spaces.


### Statements and control flow

Python's statements include:


The assignment statement (=) binds a name as a reference to a separate, dynamically allocated object. Variables may subsequently be rebound at any time to any object. In Python, a variable name is a generic reference holder without a fixed data type; however, it always refers to some object with a type. This is called dynamic typing—in contrast to statically-typed languages, where each variable may contain only a value of a certain type.


Python does not support tail call optimization or first-class continuations, and, according to Van Rossum, it never will. However, better support for coroutine-like functionality is provided by extending Python's generators. Before 2.5, generators were lazy iterators; data was passed unidirectionally out of the generator. From Python 2.5 on, it is possible to pass data back into a generator function; and from version 3.3, it can be passed through multiple stack levels.


### Expressions

Python's expressions include:


In Python, a distinction between expressions and statements is rigidly enforced, in contrast to languages such as Common Lisp, Scheme, or Ruby. This leads to duplicating some functionality. For example:


Statements cannot be a part of an expression—so list and other comprehensions or lambda expressions, all being expressions, cannot contain statements. A particular case is that an assignment statement such as a = 1 cannot form part of the conditional expression of a conditional statement.


### Methods

Methods on objects are functions attached to the object's class; the syntax instance.method(argument) is, for normal methods and functions, syntactic sugar for Class.method(instance, argument). Python methods have an explicit self parameter to access instance data, in contrast to the implicit self (or this) in some other object-oriented programming languages (e.g., C++, Java, Objective-C, Ruby). Python also provides methods, often called dunder methods (due to their names beginning and ending with double-underscores), to allow user-defined classes to modify how they are handled by native operations including length, comparison, in arithmetic operations and type conversion.


### Typing

Python uses duck typing and has typed objects but untyped variable names. Type constraints are not checked at compile time; rather, operations on an object may fail, signifying that it is not of a suitable type. Despite being dynamically typed, Python is strongly typed, forbidding operations that are not well-defined (for example, adding a number to a string) rather than silently attempting to make sense of them.


Python allows programmers to define their own types using classes, most often used for object-oriented programming. New instances of classes are constructed by calling the class (for example, SpamClass() or EggsClass()), and the classes are instances of the metaclass type (itself an instance of itself), allowing metaprogramming and reflection.


Before version 3.0, Python had two kinds of classes (both using the same syntax):  old-style and new-style; current Python versions only support the semantics of the new style.


Python supports optional type annotations. These annotations are not enforced by the language, but may be used by external tools such as mypy to catch errors. Mypy also supports a Python compiler called mypyc, which leverages type annotations for optimization.


1.33333


### Arithmetic operations

Python has the usual symbols for arithmetic operators (+, -, *, /), the floor division operator // and the modulo operation % (where the remainder can be negative, e.g. 4 % -3 == -2). It also has ** for exponentiation, e.g. 5**3 == 125 and 9**0.5 == 3.0, and a matrix‑multiplication operator @ . These operators work like in traditional math; with the same precedence rules, the operators infix (+ and - can also be unary to represent positive and negative numbers respectively).


The division between integers produces floating-point results. The behavior of division has changed significantly over time:


In Python terms, / is true division (or simply division), and // is floor division. / before version 3.0 is classic division.


Rounding towards negative infinity, though different from most languages, adds consistency. For instance, it means that the equation (a + b)//b == a//b + 1 is always true. It also means that the equation b*(a//b) + a%b == a is valid for both positive and negative values of a. However, maintaining the validity of this equation means that while the result of a%b is, as expected, in the half-open interval  when b is negative.


Python provides a round function for rounding a float to the nearest integer. For tie-breaking, Python 3 uses round to even: round(1.5) and round(2.5) both produce 2. Versions before 3 used round-away-from-zero: round(0.5) is 1.0, round(-0.5) is −1.0.


Python allows Boolean expressions with multiple equality relations in a manner that is consistent with general use in mathematics. For example, the expression a < b < c tests whether a is less than b and b is less than c. C-derived languages interpret this expression differently: in C, the expression would first evaluate a < b, resulting in 0 or 1, and that result would then be compared with c.


Python uses arbitrary-precision arithmetic for all integer operations. The Decimal type/class in the decimal module provides decimal floating-point numbers to a pre-defined arbitrary precision and several rounding modes. The Fraction class in the fractions module provides arbitrary precision for rational numbers.


Due to Python's extensive mathematics library, and the third-party library NumPy that further extends the native capabilities, it is frequently used as a scientific scripting language to aid in problems such as numerical data processing and manipulation.


### Function syntax


Functions are created in Python using the def keyword. In Python, you define the function as if you were calling it, by typing the function name and then the attributes required. Here is an example of a function that will print whatever is given:

If you want the attribute to have a set value if no value is given, use the variable-defining syntax inside the function definition.


## Programming examples

"Hello, World!" program:


Program to calculate the factorial of a positive integer:


## Libraries

Python's large standard library provides tools suited to many tasks and is commonly cited as one of its greatest strengths. For Internet-facing applications, many standard formats and protocols such as MIME and HTTP are supported. It includes modules for creating graphical user interfaces, connecting to relational databases, generating pseudorandom numbers, arithmetic with arbitrary-precision decimals, manipulating regular expressions, and unit testing.


Some parts of the standard library are covered by specifications—for example, the Web Server Gateway Interface (WSGI) implementation wsgiref follows PEP 333—but most are specified by their code, internal documentation, and test suites. However, because most of the standard library is cross-platform Python code, only a few modules need altering or rewriting for variant implementations.


As of 22 February 2025, the Python Package Index (PyPI), the official repository for third-party Python software, contains over 610,902 packages with a wide range of functionality, including:


## Development environments

Most Python implementations (including CPython) include a read–eval–print loop (REPL), permitting them to function as a command line interpreter for which users enter statements sequentially and receive results immediately.


Python also comes with an Integrated development environment (IDE) called IDLE, which is more beginner-oriented.


Other shells, including IDLE and IPython, add further abilities such as improved auto-completion, session state retention, and syntax highlighting.


As well as standard desktop integrated development environments including PyCharm, IntelliJ Idea, Visual Studio Code etc, there are web browser-based IDEs, including SageMath, for developing science- and math-related programs; PythonAnywhere, a browser-based IDE and hosting environment; and Canopy IDE, a commercial IDE emphasizing scientific computing.


## Implementations

### Reference implementation

CPython is the reference implementation of Python. It is written in C, meeting the C89 standard (Python 3.11 uses C11) with several select C99 features. CPython includes its own C extensions, but third-party extensions are not limited to older C versions—e.g. they can be implemented with C11 or C++. CPython compiles Python programs into an intermediate bytecode which is then executed by its virtual machine. CPython is distributed with a large standard library written in a mixture of C and native Python, and is available for many platforms, including Windows (starting with Python 3.9, the Python installer deliberately fails to install on Windows 7 and 8; Windows XP was supported until Python 3.5) and most modern Unix-like systems, including macOS (and Apple M1 Macs, since Python 3.9.1, with experimental installer), with unofficial support for VMS. Platform portability was one of its earliest priorities. (During Python 1 and 2 development, even OS/2 and Solaris were supported, but support has since been dropped for many platforms.)


All current Python versions (i.e. since 3.7) only support operating systems with multi-threading support.


### Other implementations

All alternative implementations have at least slightly different semantics (e.g. may have unordered dictionaries, unlike all current Python versions), e.g. with the larger Python ecosystem, such as with supporting the C Python API of with PyPy:


### No longer supported implementations

Other just-in-time Python compilers have been developed, but are now unsupported:


### Cross-compilers to other languages

There are several compilers/transpilers to high-level object languages, with either unrestricted Python, a restricted subset of Python, or a language similar to Python as the source language:


Specialized:


Older projects (or not to be used with Python 3.x and latest syntax):


### Performance

Performance comparison of various Python implementations on a non-numerical (combinatorial) workload was presented at EuroSciPy '13. Python's performance compared to other programming languages is also benchmarked by The Computer Language Benchmarks Game.


## Development

Python's development is conducted largely through the Python Enhancement Proposal (PEP) process, the primary mechanism for proposing major new features, collecting community input on issues, and documenting Python design decisions. Python coding style is covered in PEP 8. Outstanding PEPs are reviewed and commented on by the Python community and the steering council.


Enhancement of the language corresponds with the development of the CPython reference implementation. The mailing list python-dev is the primary forum for the language's development. Specific issues were originally discussed in the Roundup bug tracker hosted at by the foundation. In 2022, all issues and discussions were migrated to GitHub. Development originally took place on a self-hosted source-code repository running Mercurial, until Python moved to GitHub in January 2017.


CPython's public releases come in three types, distinguished by which part of the version number is incremented:


Many alpha, beta, and release-candidates are also released as previews and for testing before final releases. Although there is a rough schedule for each release, they are often delayed if the code is not ready. Python's development team monitors the state of the code by running the large unit test suite during development.


The major academic conference on Python is PyCon. There are also special Python mentoring programs, such as PyLadies.


Python 3.12 removed wstr meaning Python extensions need to be modified, and 3.10 added pattern matching to the language.


Python 3.12 dropped some outdated modules, and more will be dropped in the future, deprecated as of 3.13; already deprecated array 'u' format code will emit DeprecationWarning since 3.13 and will be removed in Python 3.16. The 'w' format code should be used instead. Part of ctypes is also deprecated and http.server.CGIHTTPRequestHandler will emit a DeprecationWarning, and will be removed in 3.15. Using that code already has a high potential for both security and functionality bugs. Parts of the typing module are deprecated, e.g. creating a typing.NamedTuple class using keyword arguments to denote the fields and such (and more) will be disallowed in Python 3.15.


## API documentation generators

Tools that can generate documentation for Python API include pydoc (available as part of the standard library), Sphinx, Pdoc and its forks, Doxygen and Graphviz, among others.


## Naming

Python's name is derived from the British comedy group Monty Python, whom Python creator Guido van Rossum enjoyed while developing the language. Monty Python references appear frequently in Python code and culture; for example, the metasyntactic variables often used in Python literature are spam and eggs instead of the traditional foo and bar. The official Python documentation also contains various references to Monty Python routines. Users of Python are sometimes referred to as "Pythonistas".


The prefix Py- is used to show that something is related to Python. Examples of the use of this prefix in names of Python applications or libraries include Pygame, a binding of Simple DirectMedia Layer to Python (commonly used to create games); PyQt and PyGTK, which bind Qt and GTK to Python respectively; and PyPy, a Python implementation originally written in Python.


## Popularity

Since 2003, Python has consistently ranked in the top ten most popular programming languages in the TIOBE Programming Community Index where as of December 2022 it was the most popular language (ahead of C, C++, and Java). It was selected as Programming Language of the Year (for "the highest rise in ratings in a year") in 2007, 2010, 2018, and 2020 (the only language to have done so four times as of 2020).


Large organizations that use Python include Wikipedia, Google, Yahoo!, CERN, NASA, Facebook, Amazon, Instagram, Spotify, and some smaller entities like Industrial Light & Magic and ITA. The social news networking site Reddit was written mostly in Python. Organizations that partially use Python include Discord and Baidu.


## Uses

Python can serve as a scripting language for web applications, e.g. via mod_wsgi for the Apache webserver. With Web Server Gateway Interface, a standard API has evolved to facilitate these applications. Web frameworks like Django, Pylons, Pyramid, TurboGears, web2py, Tornado, Flask, Bottle, and Zope support developers in the design and maintenance of complex applications. Pyjs and IronPython can be used to develop the client-side of Ajax-based applications. SQLAlchemy can be used as a data mapper to a relational database. Twisted is a framework to program communications between computers, and is used (for example) by Dropbox.


Libraries such as NumPy, SciPy and Matplotlib allow the effective use of Python in scientific computing, with specialized libraries such as Biopython and Astropy providing domain-specific functionality. SageMath is a computer algebra system with a notebook interface programmable in Python: its library covers many aspects of mathematics, including algebra, combinatorics, numerical mathematics, number theory, and calculus. OpenCV has Python bindings with a rich set of features for computer vision and image processing.


Python is commonly used in artificial intelligence projects and machine learning projects with the help of libraries like TensorFlow, Keras, Pytorch, scikit-learn and the Logic language ProbLog. As a scripting language with a modular architecture, simple syntax, and rich text processing tools, Python is often used for natural language processing.


The combination of Python and Prolog has proved to be particularly useful for AI applications, with Prolog providing knowledge representation and reasoning capabilities. The Janus system, in particular, exploits the similarities between these two languages,
in part because of their use of dynamic typing, and the simple recursive nature of their
data structures. Typical applications of this combination include  natural language processing, visual query
answering, geospatial reasoning, and handling of semantic web data.
The Natlog system, implemented in Python, uses Definite Clause Grammars (DCGs) as prompt generators for text-to-text generators like GPT3 and text-to-image generators like DALL-E or Stable Diffusion.


Python can also be used for graphical user interface (GUI) by using libraries like Tkinter.


Python has been successfully embedded in many software products as a scripting language, including in finite element method software such as Abaqus, 3D parametric modelers like FreeCAD, 3D animation packages such as 3ds Max, Blender, Cinema 4D, Lightwave, Houdini, Maya, modo, MotionBuilder, Softimage, the visual effects compositor Nuke, 2D imaging programs like GIMP, Inkscape, Scribus and Paint Shop Pro, and musical notation programs like scorewriter and capella. GNU Debugger uses Python as a pretty printer to show complex structures such as C++ containers. Esri promotes Python as the best choice for writing scripts in ArcGIS. It has also been used in several video games, and has been adopted as first of the three available programming languages in Google App Engine, the other two being Java and Go.


Many operating systems include Python as a standard component. It ships with most Linux distributions, AmigaOS 4 (using Python 2.7), FreeBSD (as a package), NetBSD, and OpenBSD (as a package) and can be used from the command line (terminal). Many Linux distributions use installers written in Python: Ubuntu uses the Ubiquity installer, while Red Hat Linux and Fedora Linux use the Anaconda installer. Gentoo Linux uses Python in its package management system, Portage.


Python is used extensively in the information security industry, including in exploit development.


Most of the Sugar software for the One Laptop per Child XO, developed at Sugar Labs as of 2008, is written in Python. The Raspberry Pi single-board computer project has adopted Python as its main user-programming language.


LibreOffice includes Python and intends to replace Java with Python. Its Python Scripting Provider is a core feature since Version 4.0 from 7 February 2013.


## Languages influenced by Python

Python's design and philosophy have influenced many other programming languages:


Python's development practices have also been emulated by other languages. For example, the practice of requiring a document describing the rationale for, and issues surrounding, a change to the language (in Python, a PEP) is also used in Tcl, Erlang, and Swift.


## See also

## References

### Sources

## Further reading

## External links

