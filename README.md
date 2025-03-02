# Keywords
## climb
    Increments the current memory location by 1.
## fall
    Decrements the current memory location by 1.
## wind
    Takes an address, copies the value from the current memory location to the provided location.
## dash
    Sets the current memory location to the provided address.
## jump
    Sets a jump marker with value equal to the provided number.
## spring
    Moves the program execution pointer to the jump marker with the value equal to the provided number.
## spike
    Skips all instructions until the jump instruction with the value equal to the provided number.
## spinner
    Built-in rng keyword. Has a 1/3 chance to set the current memory value to 1; otherwise sets it to 0.

# Numbers
    Any of these can be used interchangeably with all keywords that take an argument.
## smotsinary
    like binary, but the character '7' represents 0 and the character '8' represents 1
## references
    $number refers to the value stored at the memory address number.
## user input with @madeline
    @madeline prompts the user for input, and has the value of the number they input.
