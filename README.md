# Keywords
## climb
    Increments the current memory location by 1.
## fall
    Decrements the current memory location by 1.
## crumble
    Sets the current memory location to a given number.
## run
    Outputs the current memory value.
## retry
    Same as run, but doesn't print a newline afterwards.
## wind
    Takes an address, copies the value from the current memory location to the provided location.
## dash
    Sets the current memory location to the provided address.
## jump
    Sets a jump marker with value equal to the provided number.
## spring
    Moves the program execution pointer to the jump marker with the value equal to the provided number.
    Does nothing instead if the current memory value is 0.
## spike
    Does nothing unless the current memory value is 0.
    Skips all instructions until the jump instruction with the value equal to the provided number.
## spinner
    Built-in rng keyword. Has a 1/3 chance to set the current memory value to 1; otherwise sets it to 0.
## smots5
    Terminates the program.
## triggerspike
    If the current memory value is equal to the given number, do nothing, else skips all instructions until the given jump marker
## trigspike
    Alias for triggerspike.
## campaign
    Takes an agrument of a path to a smotslang file and runs it.
## debug
    Sets the program to output numbers
## reload
    Sets the program to output characters

# Numbers
    Any of these can be used interchangeably with all keywords that take an argument.
## smotsinary
    like binary, but the character '7' represents 0 and the character '8' represents 1
## references
    $number refers to the value stored at the memory address number.
## user input with @madeline
    @madeline prompts the user for input, and has the value of the number they input.
## numbers
    Smotsinary can be hard to work with, so if you put a `^` before a base 10 number, it converts it to smotsinary for you!
## chars
    Like numbers but if you put a `'` before a character to convert it into smotsinary.
> [!NOTE]
> You can't use this method to get characters like spaces however!

# File System
Smotslang has a special memory slot for holding file paths, to set this slot use the state keyword.\
`state C:\Users\Admin\Downloads\smotslang\examples\meow.txt` loads meow.txt into memory.
You can also use the `badeline` keyword to open a file prompt, setting the current file to the selection.
> [!NOTE]
> The default value of the file memory is smotslang's index.js, so be careful!
# Reading Files
To read from the open file, use @tas.\
`@tas` gets the nth byte of a file where n is the current memory value.\
`climb crumble @tas` stores the second byte of meow.txt to memory.\
<br/>
To get the length of the file use `@recordcount`
# Comments
    Denoted by wrapping the comment in --
    Example: -- smots gaming --  (Including the spaces is important!)
