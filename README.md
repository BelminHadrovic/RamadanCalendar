<h1>Vaktija Console Application</h1>

This is a simple console application that calculates and displays prayer times (vaktija) for a given date range. The application uses the Vaktija.Models namespace to work with date intervals.

<h2>Requirements</h2>

.NET Core 3.1 or later

<h2>How to Use</h2>

Clone the repository or download the source code.

Build the project using the following command:

dotnet build

Run the application:

dotnet run

The application will prompt you to enter the date range in the format dd/MM/yyyy. Follow the on-screen instructions and input the start and end dates for which you want to calculate the prayer times.

The application will then load the necessary data and display the calculated prayer times for each day in the specified date range.

Press any key to exit the application after viewing the results.

<h2>Code Overview</h2>

<br>**Main**</br>
The entry point of the application. It calls the unosKorisnika method to get the user input for the date range and then passes it to the prikazVaktije method.

<br>**unosKorisnika**</br>
This method prompts the user to enter the start and end dates for the date range. It validates the input and returns an IntervalDatuma object containing the specified date range.

<br>**prikazVaktije**</br>
This method creates a new instance of KalendarVaktija with the provided date range and awaits the popuniVaktiju method to load the necessary data. After loading the data, it displays the prayer times using the Console.WriteLine method.

<br>**unosDatuma**</br>
A utility method to parse user input and validate it as a valid date in the format dd/MM/yyyy.
