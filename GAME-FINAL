#include <cstdlib> // Loads libraries
#include <time.h>  // --
#include <iostream> // --

using namespace std; // Makes functions with the same names within different libraries distinguishable

int PickCard() { // The function that generates a random number between 1 and 13
  
   
  int x; // Placehodler int to hold the card value
  x = (rand()%13)+1; // The random number generator
  
  
  return x; // Returns the result of the random number generator
  
}



main() { // Main function
  
	int cash = 0; // Makes the cash variable
  
	CorrectGuess: // Marker to go to later so that the cash variable doesn't get reset to 0
  
	srand((unsigned)time(NULL)); // Seeds the random number generator
  
    	int card1 = PickCard(); // Declares a new variable called card1 with a value decided by the random number generator
  
    	cout << "Your number is" << "\n"; // The following lines print the text in the command line
  
    	cout << card1 << "\n"; // Prints value of card1
    
    	cout << "Higher or Lower? 1 for Higher, 2 for Lower" << "\n"; // --
    
    	int card2 = PickCard(); // Declares a new variable called card2 with a value decided by the random number generator
  
    	int guess; // Declares a new variable to hold the players guess

    	cin >> guess; // Whatever the player inputs into the command line is held as the value to the variable guess
    
		if ( guess == 1 ){ // This checks to see what the players guess was, the value of '1' means the player guessd higher
			if ( card2 > card1 ){ // This checks if the players guess was correct
				cash += 50; // adds 50 to the value of the variable 'cash' 
				
				cout << "You guessed higher. The number was: " << card2 << ". Well Done!" "\n" "\n"; // Prints text to let the player know that their guess was correct

				goto CorrectGuess; // Sends the program back to the 'CorrectGuess' marker
				
				}
					else cout << "Game over, the number was: " << card2 << "\n" << "You finished the game with " << cash << " Dollars" "\n" "\n"; // If the player's guess was wrong, prints game over text and displays how much cash they made
				}
    
					if ( guess == 2 ){ // This checks to see if the players guess was lower, value of 2
						if ( card2 < card1 ){ // This checks if the players guess was correct
							cash += 50; // adds 50 to the value of the variable 'cash'
				
							cout << "You guessed lower. The number was: " << card2 << ". Well Done!" "\n" "\n"; // Prints text to let the player know that their guess was correct
					
							goto CorrectGuess; // Sends the program back to the 'CorrectGuess' marker
					
							}
								else cout << "Game over, the number was: " << card2 << "\n" << "You finished the game with " << cash << " Dollars" "\n" "\n"; // If the player's guess was wrong, prints game over text and displays how much cash they made
							}

	  
}
