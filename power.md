# Power-on and power-off

## Scenario: User turned on calculator with history stored
  
  Given user has turned on calculator and calculation history present in file storage.
  When I press on
  Then I see the calculation history in history tab.
  
## Scenario: User turned on calculator with no history stored
  
  Given user has turned on calculator and calculation history not present in file
  storage.
  When I press on
  Then I see the new calculator with no history tab.
  
## Scenario: User turned off calculator after clearing history tab
  
  Given user has turned off calculator.
  When user deletes history of calculation and turned off calculator
  Then calculator go to off state after deleting all history.
  
## Scenario: User turned off calculator without clearing history tab
  
  Given user has turned off calculator.
  When user turned off calculator and history tab contains data
  Then calculator stores history in file storage system and turns off.
  When user press off and history tab does not contain data
  Then calculator turns off without storing history in file storage system.
