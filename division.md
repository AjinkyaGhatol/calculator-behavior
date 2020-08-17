# Multiplication

## Scenario: Multiplication of two positive numbers
  
  Given user has turned on calculator.
  When I type in positive number and I press multiply and I type in Positive number
  and I press equal
  Then I see the multiplication in result.

## Scenario: Multiplication of two negative numbers
  
  Given user has turned on calculator.
  When I type in first negative number and I press multiply and I type in second
  negative number and I press equal
  Then I see the multiplication in result.
  
## Scenario: First operand is positive and second operand is negative

  Given user has turned on calculator. ( user input: 6*(-7)=)

  When I type in positive number and I press multiply and I press open bracket and
  I type in negative number and i press close bracket and I press equal
  Then calculator will multiply two numbers. Output for given user input: -42
  
## Scenario: First operand is negative and second operand is positive
  
  Given user has turned on calculator. ( user input: -7*6=)

  When I type in negative number and I press multiply and I type in positive number
  and I press equal
  Then calculator will multiply two numbers. Output for given user input: -42
  
## Scenario: User pressed multiply more than once
  
  Given user has turned on calculator.

  When I type in number and I press multiply more than once  
  Then calculator will consider single multiply.
  
## Scenario: Multiplication of fraction
  
  Given user has turned on calculator.

  When I type in first fraction number and I press multiply and I type in second
  fraction number and press equal
  Then I see the multiplication with fraction in result.
  
## Scenario: Multiplication of decimals
  
  Given user has turned on calculator.

  When I type in first decimal number and I press multiply and I type in second
  decimal number and press equal
  Then I see the multiplication in result.
  
## Scenario: Multiplication of more than two numbers
  
  Given user has turned on calculator.
  
  When I try to multiply more than two numbers
  Then I see the multiplication from left to right in result.
  
## Scenario: Multiplication is out of range
  
  Given user has turned on calculator.
  
  When I type in number and I press multiply and I type in number
  and I press equal and result is out of range
  Then calculator display result with power 10 and user can see whole result
  by scroll in horizontal.
  
## Scenario: User pressed another operator after pressing multiplyyyyy operator
  
  Given user has turned on calculator. ( user input: 6*+)
  
  When User pressed another operator after pressing multiply operator
  Then calculator replace multiply operator with new operator. Output for given
  user input: 6+
