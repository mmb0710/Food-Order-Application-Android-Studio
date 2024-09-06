# Recipe Search Application

## Overview
The **Recipe Search Application** is an Android-based application designed to search, display, and manage recipes by interacting with the Spoonacular API. Users can search for recipes, view detailed information about a selected recipe, and save their favorite recipes to a local database for later viewing or deletion.

This project was developed as part of the **CST2335 Graphical Interface Programming** course, focusing on implementing Android UI components, database interactions, and network requests using the Volley library.

## Features
- **Recipe Search**: Allows users to search for recipes by name using the Spoonacular API.
- **Recipe Details**: Displays detailed information about selected recipes, including images, summaries, and source URLs.
- **RecyclerView for Recipe List**: Displays the search results and saved recipes in a scrollable list using RecyclerView.
- **Save Recipes**: Users can save favorite recipes to a local SQLite database.
- **Delete Recipes**: Users can delete recipes from the local database.
- **Volley for API Requests**: Utilizes the Volley library to retrieve recipe data from the Spoonacular API.
- **Notifications**: Includes Toasts, Snackbars, and AlertDialogs for user interactions.
- **EditText and Button**: Allows users to input recipe names to search and execute actions via buttons.
- **SharedPreferences**: Saves the last search term for future app launches.
- **Multiple Language Support**: Supports at least one additional language.
- **Professional UI**: The app features a clean and user-friendly interface with properly aligned and professional-looking GUI elements.
- **JUnit Test Cases**: Includes at least five test cases to validate UI and functionality.
- **JavaDoc Documentation**: All code is properly documented with JavaDoc comments, including a header for each file with details like author, purpose, and date of creation.

## Requirements
1. **RecyclerView**: Displays a list of recipes retrieved from the Spoonacular API and saved favorites from the local database.
2. **SQLite Database**: Stores favorite recipes, enabling users to add and delete items.
3. **Volley**: Makes API requests to the Spoonacular API to search for recipes and retrieve recipe details.
4. **Toasts, Snackbars, AlertDialogs**: Provides feedback and notifications to users.
5. **EditText and Buttons**: Provides input fields for entering search terms and buttons for actions like searching and saving recipes.
6. **SharedPreferences**: Remembers the last search term the user entered for convenience on future app launches.
7. **Localization**: Supports at least one additional language.
8. **Professional UI**: Ensures a clean, user-friendly layout.
9. **JavaDoc Comments**: Includes proper documentation of all methods and classes.
10. **Test Cases**: At least five test cases for interface and functionality.

## Getting Started

### Prerequisites
- **Android Studio**: Download and install [Android Studio](https://developer.android.com/studio).
- **Spoonacular API Key**: Get your API key from [Spoonacular](https://spoonacular.com/food-api/console#Dashboard).
  
##API Information
Recipe Search URL:

https://api.spoonacular.com/recipes/complexSearch?query=XXXXX&apiKey=YYYYY
Replace XXXXX with the recipe search term and YYYYY with your Spoonacular API key.

Recipe Details URL:

https://api.spoonacular.com/recipes/ID/information?apiKey=YYYYY
Replace ID with the recipe ID from the search results and YYYYY with your API key.

### Usage
Search for a Recipe:

Enter the recipe name in the search field and press the "Search" button.
The app will display the search results in a RecyclerView.

## View Recipe Details:

Tap on a recipe from the search results to view its details, including the image, summary, and source URL.

## Save a Recipe:

Press the "Save" button in the recipe details to store the recipe in your local favorites database.

## View Saved Recipes:

Press the "View Favorites" button to see a list of saved recipes from the local database.

## Delete a Recipe:

Select a saved recipe and press the "Delete" button to remove it from your favorites list.

## Search Term Memory:

The app saves the last searched term using SharedPreferences, which is loaded when the app is reopened.

