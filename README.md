# FootballClubsDatabase

Detailed Project Structure
MainActivity.kt
This is the entry point of the application. It contains the navigation logic to switch between different screens based on user actions.

AddLeaguesScreen.kt
This screen is displayed when the user clicks on Add Leagues to DB.
It hardcodes the details of several football leagues and saves them into the local SQLite database using Room Library.

SearchClubsByLeagueScreen.kt
This screen is displayed when the user clicks on Search for Clubs By League.
Contains a textbox for inputting the league name and two buttons: Retrieve Clubs and Save Clubs to Database.
On clicking Retrieve Clubs, it fetches and displays all clubs in the specified league using TheSportsDB API.
On clicking Save Clubs to Database, it saves the fetched club details into the local SQLite database.

SearchClubsScreen.kt
This screen is displayed when the user clicks on Search for Clubs.
Contains a textbox for inputting a search string and a Search button.
It searches the local SQLite database for clubs whose name or league contains the search string and displays the results.
Displays club details along with their logo images.

Data Directory
Contains Room database entities, Data Access Objects (DAOs), and repository classes to manage data storage and retrieval.

Setup Instructions
Clone the Repository: Use git clone <repository_url> to clone the repository to your local machine.
Open in Android Studio: Open Android Studio and select Open an existing Android Studio project, then navigate to the cloned repository.
Sync Gradle: Ensure all dependencies are synced by clicking Sync Now when prompted by Android Studio.
Run the Application: Select an emulator or connect a physical device, then click Run to build and launch the application.

Development Guidelines
Kotlin: Ensure all new code is written in Kotlin.
Jetpack Compose: Follow Compose guidelines for UI development, avoiding traditional Views.
Room Library: Use Room for all database operations, adhering to best practices for database management.

API Integration
TheSportsDB API: Use the API to fetch league and club data. Ensure API requests are handled asynchronously to avoid blocking the main thread.
Error Handling: Implement robust error handling for API requests and database operations to ensure a smooth user experience.

Contributions
Fork the Repository: Click on the Fork button to create a personal copy of the repository.
Make Changes: Clone your forked repository and make changes.
Pull Request: Push changes to your fork and create a pull request to the original repository.
