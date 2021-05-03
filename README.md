# Excellent Developer

This repository is a guide on the way to becoming an excellent developer. Most developers know the development tools and technologies they use well, but rarely do they know the details, with fatal consequences for their clients and collegues sometimes. E.g. in Python `everything is an object` and so is this function definition:

```Python
def is_first_letter_an_a(somestr):
    return len(somestr) > 0 and somestr[0] in [‘a‘, ‘A‘]
```

Well, where is the object you may ask. It’s the Python interpreter that creates an object out of this definition. An object to which the surrounding code has access through the function name by the way.   From this knowledge it follows that functions can be treated like any other objects in Python, in particular they can be assigned to variables, passed as arguments or modified. For example:

```Python
def get_hello_world():
    return „Hello, World!“

def get_hello_dear():
    return „Hello, Dear!“

get_hello_world.__code__ = get_hello_dear.__code__
print( get_hello_world() )
```

What output do you expect here? Go ahead and inspect the function object further using the usual methods.

## How does this guide help?
This guide is not a course that demonstrates, but asks questions and tasks to be answered and worked on you own. Thus, in the end, not only is the knowledge firmly learned, but also the ability to teach oneself knowledge from a wide variety of sources and the often overlooked official documentation and standards is acquired.

## How does this guide work?
This guide is structured in steps, with each step building on the knowledge of the previous steps. Each step contains a note on the approximate processing time frame, so that the processor does not get lost in research or spend too long on a question or task before another solution path is taken.

## How do I submit my solution?
Solutions to the individual steps are to be submitted via pull request. The solution files should be located in a folder with the step number and in a folder with the GitHub user name. For example, the solutions of `astzweig` for step `1.A.` are located in the folder `1-A/astzweig` (dots are replaced by hyphens) relative to this repository.
Solutions to questions shall be answered in markdown files.

## Existing Steps

| Step | Topics |
| --- | --- |
| [1.A][step_1] | Computer processes, Threads and IPC |

[step_1]: 1-A_Step.md
