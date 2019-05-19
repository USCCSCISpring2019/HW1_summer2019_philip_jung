# HW1_summer2019_philip_jung
## Has 5 Java classes

### Main.java is the entry point
Requests a filename from the User
And calls the static function Readfile.read( ) to try to collect the city information from the file.
After a successful read, initializes Menu and runs Menu.app()

### Readfile.java has a single static function with signature boolean read(ArrayList<City>, String fileName)
if successfully read City information and stored in ArrayList<City> then returns true
else, prints out the appropriate error, closes the scanner(File) and returns false

### City.java is the class for cities
holds all private data and public getters for City class
currently, no setter functions (in constructor only)
uses a private custom parser function that throws a new MyException if error in data

### MyException.java is my custom exception class
This was made in order to have more control of the error messages that will displayed

### Menu.java is where the program is where the action takes place
Menu's constructor takes two args, ArrayList<City> and a reference to Scanner(System.in)
This was done so that the System.in will be closed only once at the end of the program (in Main)
Other than that, this program just responds to integer inputs from the User and just displays text



