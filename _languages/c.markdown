---
layout: language
icon: icon-c

Language: C
Language_Description: General purpose, low-level programming language.

Data_Types:
- Type: int
  Description: Declares an integer.
  Syntax: int variable_name;

- Type: float
  Description:  Declares a variable that's able to harness the power of decimals (accurate up to 7 digits).
  Syntax: float variable_name;

- Type: double
  Description: Same as float, but is more exact (acurate up to 15 digits).
  Syntax: double variable_name;

- Type: char
  Description: 8 bit data type that usually contains characters.
  Syntax: char variable_name;

Structures:
- Type: if
  Description: Executes code if the following statement is true.
  Syntax: if(statement) {code}
  Example: if(x>5) {code}
  Example_Description: Code will only be executed if the variable x is greater than 5.

- Type: else
  Description: Follows an if block and will be executed if the if block isn't.
  Syntax: else {code}

- Type: else if
  Description: Follows an if block and will be executed if the previous if block wasn't executed and the new parameters are met.
  Syntax: else if (statement) {code}
  Example: else if (x==5) {code}
  Example_Description: Executes when previous if block doesn't and only if x equals 5.

- Type: while
  Description: Repeats code as long as statement remains true.
  Syntax: while (statement) {code}
  Example: while (x>5) {code}
  Example_Description: Code will only execute if x is greater than 5 and will keep looping until x isn't greater than 5.

- Type: do while
  Description: Code executes once and then statement is tested.  If statement remains true the do while will keep looping.
  Syntax: do while (statement) {code}
  Example: do while (x>5) {code}
  Example_Description: Code will execute once and then test if x is greater than 5.  If it is then it'll loop, if not it'll move on.

- Type: for
  Description: Loops as long as the stated conditions are met.
  Syntax: for (variable, statement, increment) {code}
  Example: for (int x=0; x>5, x++) {code}
  Example_Description: Evaluates 'x' and loops if x is greater than 5.  After each execution the value of x will increase by '+1'.

- Type: switch
  Description: Allows specific code to be used. Variable used must be an integer and the 'vars' must be constant. The switch will jump to the first case that's equal to your stated variable and do the rest of the codes from there (so it'll skip everything before the first case used).  If none of the cases are equal to your variable then it'll only execute the last section of code (the code following 'default').
  Syntax: |
          switch (variable)
          {case var1: code;
          case var2: code;
          default: code; }
  Example: |
          int x = 5
          var1 = 4
          var2 = 5
          switch (x)
            {case var1: code;
            case var2: code:
            default: code; }
  Example_Description: This switch would skip the first line of code and execute everything after that.

User_Interface:
- Type: scanf
  Description: Retrieves from stdin and assigns input to a variable. If you're inputting a string don't add the '&.'
  Syntax: scanf (input, &variable);
  Example: scanf (10, x)
  Example_Description: This would import a value of 10 for 'x.'

- Type: printf
  Description: Displays to stdout.
  Syntax: printf ("text");
  Example: printf (x);
  Example_Description: Displays the value of 'x.'

Comments:
- Type: Single Line
  Syntax: //comments

- Type: Block
  Syntax: "*/many comments/*"


Hello_World:
- Type: Example
  Example: |-
    #include<stdio.h>
    main()
    {
      printf("Hello World");
    }
---
