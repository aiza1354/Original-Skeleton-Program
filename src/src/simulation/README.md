* Observations:
  * It should handle undefined simulation input with appropriate message. TRY-CATCH
  * In constructors, you should add this. to refer to one single attributes (if there are multiple attributes with the same name).
  * For Display Detail and Display Area Detail we can DEFINITELY reuse code and make it more efficient by combing some of their features. 
  * We can definitely add more methods to make them reusable.
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
  * 