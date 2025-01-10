# Dog-adoption
Overview
The Contoso PetFriends application is a console-based program designed to manage and display information about pets available at a fictional pet adoption center. The program provides users with a menu-driven interface to view pet details and search for dogs based on specified characteristics.

Features
Pet Information Management:

Stores runtime data about pets, including species, ID, age, physical description, personality, nickname, and suggested donation.
Provides sample data for demonstration purposes.
Menu Options:

Option 1: List all current pet information.
Option 2: Display dogs matching a specified physical or personality characteristic.
Data Validation:

Ensures suggested donations are valid decimal values. Defaults to $45.00 if the value is invalid.
How It Works
Initialization:

The program initializes a 2D array ourAnimals to store up to 8 pets. Each pet has the following attributes:
ID
Species
Age
Nickname
Physical description
Personality description
Suggested donation
Sample pet data is added for demonstration.
User Interaction:

Users interact with the application via a menu system:
Enter 1 to view all pet information.
Enter 2 to search for dogs with specific characteristics.
Type Exit to close the application.
Data Display:

For Option 1, the program loops through the ourAnimals array and displays all non-empty entries.
For Option 2, the program prompts the user to enter a desired characteristic, searches the combined physical and personality descriptions of all dogs, and displays matching results.
Search Functionality:

Searches only for dogs (Species: dog).
Matches the user-provided characteristic with the concatenated descriptions.
Code Structure
Variables:

ourAnimals: 2D array to store pet data.
maxPets: Maximum number of pets supported (8).
Other variables for temporary data storage and user input.
Sample Data Setup:

Populates the ourAnimals array with predefined pet data using a switch statement.
Menu System:

Implements a do-while loop to display the menu and process user input.
Error Handling:

Uses decimal.TryParse to validate donation values.
Search Logic:

Compares user input to combined pet descriptions for matching results.
Usage Instructions
Run the Program:

Launch the application in a C# environment (e.g., Visual Studio or .NET CLI).
Navigate the Menu:

Enter 1 to list all pets.
Enter 2 to search for dogs based on characteristics.
Type Exit to terminate the application.
Example Search:

For a dog that loves hugs, enter "hugs" when prompted to search for a characteristic.
