Displaying the data:
    In order to display the data within the game I have used JavaFX. Most of 
    what I did is within the code comments. In order to display the data into 
    the grid I have decided to create a grid that is double the size that the 
    user enters. Then half of that grid is used to enter squares with numbers
    and second half is used to store the constraints. When button that allows
    editing the squares is clicked the "getProblems" is being run to check if 
    there are any errors. If there are the error messages are being added to a 
    lable that is being displayed at the bottom of the screen with the game.

Editing the data:
    In order to edit data within my program I have used first of all two 
    comboBoxes. These comboBoxes allow to set the size of the grid and the 
    difficulty of it. This works by saving the number that is being chosen as 
    the size of the grid and passing it as a variable when the grid is created.
    This edits the size of the data. Then the difficulty comboBox saves as a 
    String the option that has been chosen. This is then passed as a variable
    to a method I have created in my FutoshikiPart2 that depending on which 
    option is passed to it "Easy", "Medium", "Hard" the correct numbers for 
    column constraints number and squares number is being stored. These numbers
    then are being used within the fillPuzzle method to fill the grid 
    and make it easier or harder for the user to solve. This is done by changing
    the amount of numbers filled in for the user by the game. The lower the 
    difficulty the more numbers are filled in. Where as the number of 
    constraints is opposite. The lower the difficulty the less constraints are 
    being displayed. 

    Another way of editing the data within the grid is completing the puzzle it 
    self. This is done by making each square a button that once clicked it 
    changes the number on it (and within the grid) to one higher then it was 
    before. Once it reaches the maximum number it could be it goes back to one. 
    This is done by connecting the button "setSquare" method within my 
    FutoshikiPart2. Then once the user is finished he can click the 
    "Check Configuration" button. This then runs the "isComplete" method.
    If it returns true then a congratulations pop up window opens and allows you
    to click continue. That then takes the user back to the setting page that  
    will allow him to start another game. However if the "isComplete" returns 
    false the program tells user that there is errors in his game and once he 
    clicks continue button then the pop up window closes and lets the user 
    change the grid.

Optional extras:
    My biggest optional feature is that I have used a CSS file to style the
    entire gui of the program. I have done everything that I could to make it   
    look nice and make the interface more user friendly. I have decided to use 
    an external CSS file as then I can just reference it within the code instead 
    of doing all the styling within the JavaFX. By doing this my JavaFX code 
    looks more neat and it's easier to read.

    Another feature I have decided to implement is on the front screen an 
    instructions button that opens up a pop up window that explains how to play 
    and what are the rules of the game. I have decided to do that as not 
    everyone knows how to play te game and this should make it much more clear.

    Another small additional feature that I have added is inside of my
    "fill-puzzle" method. I managed to arrange the equation 
    "(((size-1)*this.difficultyCon)/4)" for the value on how many times 
    constraints will be entered into a grid. By doing it with this equation 
    grid size 3 and 4 does not have constraints which makes it even easier. As
    the grid grows constraints in even easy mode of grid 5 6 have some 
    constraints to make it harder. By doing this grid sizes 3 and 4 have a extra
    easy mode within the easy mode. 

IMPORTANT: 

Grid size 6 on every difficulty (especially easy) needs some time to 
find one that is solvable but it works. Please give it time.

In order to run the GUI please go to the FutoshikiGUI and click Shift and F6 to 
run the file.S