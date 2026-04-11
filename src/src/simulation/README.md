* Observations:
  * It should handle undefined simulation input with appropriate message. TRY-CATCH
  * In constructors, you should add this. to refer to one single attributes (if there are multiple attributes with the same name).
  * For Display Detail and Display Area Detail we can DEFINITELY reuse code and make it more efficient by combing some of their features. 
  * We can definitely add more methods to make them reusable.
  * To quit, must enter 2 times, inefficient + less user friendly 
* 1st Method: Display Details 
  * For most of them this is the structure they follow: Example: Nest
    * using getDetails()
    * To display nests, we look through our grid which is a 2D array and during this, we loop through Nests which is a list that has the coordinates of the places that there are nests in and compare against our Grid.
    * If we find a match, then we print out "Nest".
    * Similarly, for the Ants attribute, we do the same but just use a counter to display the number of them. 
* 2nd Method: Display AREA Details
  * using getAreaDetails()     
  * This is similar to the previous method, however, instead we focus on one specific area. The user has to input a range of coordinates, and the program will display the information for that range.
  * Both Display Details and Display Area Details use the SAME function but for the latter, we use a specific range. 
  * int startRow, int startColumn, int endRow, int endColumn --> these are all initialised as 0 to begin with.
* 3rd Method: Display Cell Details
  * using getCellDetails();
  * Similar to previous ones, this time we use getCell();
  * We go into more detail here, as we learn about the typeofAnt etc.
* getIndicesofNeighbours Summary: 
  * We are making an array to have a list of the possible neighbours our ant can go to!
  * Integer rowDirection : Arrays.asList(-1, 0, 1);
    * This involves creating the ArrayList rowDirection AND looping through it, we are looping through the digits, -1, 0 and 1!
  * We create this for rowColumn too. 
  * During this we create new rows/columns which can be -1, 0 , +1 of our current column.
  * If we are not on the 0 direction, we check to see if the neighbourRow/Column is at the tbottom and top ends of the boundary. 
  * If it is we add these valuse o our neughbourList array. 
    * IF NOT: we minus one from our list to ensure that the cell that we standing on is NEVER added to this list. 