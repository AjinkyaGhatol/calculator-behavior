# Addition

## Scenario: Addition of two positive numbers
  
  Given user has turned on calculator.
  When I type in positive number and I press plus and I type in Positive number
  and I press equal
  Then I see the addition in result.

## Scenario: Addition of two negative numbers
  
  Given user has turned on calculator.
  When I type in first negative number and I press plus and I type in second
  negative number and I press equal
  Then I see the addition in result.
  
## Scenario: First operand is positive and second operand is negative

  Given user has turned on calculator. ( user input: 6+-7=)

  When I type in positive number and I press plus and I type in negative number
  and I press equal
  Then calculator will subtract two numbers. Output for given user input: -1
  
## Scenario: First operand is negative and second operand is positive
  
  Given user has turned on calculator. ( user input: -7+6=)

  When I type in negative number and I press plus and I type in positive number
  and I press equal
  Then calculator will add two numbers. Output for given user input: -1
  
## Scenario: User pressed plus more than once
  
  Given user has turned on calculator.

  When I type in number and I press plus more than once  
  Then calculator will consider single plus.
  
## Scenario: Addition of fraction
  
  Given user has turned on calculator.

  When I type in first fraction number and I press plus and I type in second
  fraction number and press equal
  Then I see the addition in result.
  
## Scenario: Addition of decimals
  
  Given user has turned on calculator.

  When I type in first decimal number and I press plus and I type in second
  decimal number and press equal
  Then I see the addition in result.
  
## Scenario: Addition of more than two numbers
  
  Given user has turned on calculator.
  
  When I try to add more than two numbers
  Then I see the addition in result.
  
## Scenario: Addition is out of range
  
  Given user has turned on calculator.
  
  When I type in number and I press plus and I type in number
  and I press equal and addition is out of range
  Then calculator display result with power 10 and user can see whole result
  by scroll in horizontal.
  
## Scenario: User pressed another operator after pressing plus operator
  
  Given user has turned on calculator. ( user input: 6+*)
  
  When User pressed another operator after pressing plus operator
  Then calculator replace plus operator with new operator. Output for given
  user input: 6*
