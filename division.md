# Division

## Scenario: Division of two positive numbers
  
  Given user has turned on calculator.
  When I type in positive number and I press divide and I type in Positive number
  and I press equal
  Then I see the division in result.

## Scenario: Division of two negative numbers
  
  Given user has turned on calculator.
  When I type in first negative number and I press divide and I type in second
  negative number and I press equal
  Then I see the division in result and result is positive number.
  
## Scenario: First operand is positive and second operand is negative

  Given user has turned on calculator. ( user input: 12/(-6)=)

  When I type in positive number and I press divide and I press open bracket and
  I type in negative number and I press close bracket and I press equal
  Then calculator will divide two numbers. Output for given user input: -2
  
## Scenario: First operand is negative and second operand is positive
  
  Given user has turned on calculator. ( user input: -12/6=)

  When I type in negative number and I press divide and I type in positive number
  and I press equal
  Then calculator will divide two numbers. Output for given user input: -2
  
## Scenario: User pressed divide more than once
  
  Given user has turned on calculator.

  When I type in number and I press divide more than once  
  Then calculator will consider single divide.
  
## Scenario: Division of fraction
  
  Given user has turned on calculator.

  When I type in first fraction number and I press divide and I type in second
  fraction number and press equal
  Then I see the division with fraction in result.
  
## Scenario: Division of decimals
  
  Given user has turned on calculator.

  When I type in first decimal number and I press divide and I type in second
  decimal number and press equal
  Then I see the division in result with decimals.
  
## Scenario: Division of more than two numbers
  
  Given user has turned on calculator.
  
  When I try to divide more than two numbers
  Then I see the division from left to right in result.
  
## Scenario: Division is out of range
  
  Given user has turned on calculator.
  
  When I type in number and I press divide and I type in number
  and I press equal and result is out of range
  Then calculator display result with power 10 and user can see whole result
  by scroll in horizontal.
  
## Scenario: User pressed another operator after pressing divide operator
  
  Given user has turned on calculator. ( user input: 6/-)
  
  When User pressed another operator after pressing divide operator
  Then calculator replace divide operator with new operator. Output for given
  user input: 6-
  note: to divide by negative number, use brackets.
