# Subtraction

## Scenario: Subtraction of two positive numbers
  
  Given user has turned on calculator.
  When I type in positive number and I press minus and I type in Positive number
  and I press equal
  Then I see the subtraction in result.

## Scenario: Subtraction of two negative numbers
  
  Given user has turned on calculator. ( user input: -6-(-6)=)
  When I type in first negative number and I press minus and I type in second
  negative number and I press equal
  Then I see the subtraction in result. Output for given user input: 0
  note: user has to use brackets for second operand to treat it as negative number otherwise Calculator converts second operand to positive number.
  
## Scenario: First operand is positive and second operand is negative

  Given user has turned on calculator. ( user input: 6-(-6)=)

  When I type in positive number and I press minus and I type in negative number
  and I press equal
  Then calculator will subtract two numbers. Output for given user input: 12
  note: user has to use brackets for second operand to treat it as negative number otherwise Calculator converts second operand to positive number.
  
## Scenario: First operand is negative and second operand is positive
  
  Given user has turned on calculator. ( user input: -7-7=)

  When I type in negative number and I press minus and I type in positive number
  and I press equal
  Then calculator will subtract two numbers. Output for given user input: -14
  
## Scenario: User pressed minus more than once
  
  Given user has turned on calculator.

  When I type in number and I press minus more than once  
  Then calculator will consider single minus.
  
## Scenario: Subtraction of fraction
  
  Given user has turned on calculator.

  When I type in first fraction number and I press minus and I type in second
  fraction number and press equal
  Then I see the subtraction in result with fraction.
  
## Scenario: Subtraction of decimals
  
  Given user has turned on calculator.

  When I type in first decimal number and I press minus and I type in second
  decimal number and press equal
  Then I see the subtraction in result with decimals.
  
## Scenario: Subtraction of more than two numbers
  
  Given user has turned on calculator.
  
  When I try to subtract more than two numbers
  Then I see the subtraction in result.
  note: subtraction is done according to precedence.
  
## Scenario: Subtraction is out of range
  
  Given user has turned on calculator.
  
  When I type in number and I press minus and I type in number
  and I press equal and subtraction is out of range
  Then calculator display result with power 10 and user can see whole result
  by scroll in horizontal.
  
## Scenario: User pressed another operator after pressing minus operator
  
  Given user has turned on calculator. ( user input: 6-+)
  
  When User pressed another operator after pressing minus operator
  Then calculator replace minus operator with new operator. Output for given
  user input: 6+
  note: user has to use brackets for second operand to treat it as negative number otherwise Calculator converts second operand to positive number.
