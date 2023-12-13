# Flash Card Component

A simple React application that displays flashcards with questions and answers. This flashcard interface where clicking on a flashcard toggles between displaying the question and its answer.

### App Component:

This is the main component of the application, which serves as the entry point.
It renders a div with the class name "App" and includes the FlashCards component.

### Questions Array:

An array containing objects representing flashcards. Each object has an id, a question, and an answer.

### FlashCards Component:

Renders a collection of flashcards using the questions array.
Manages a state variable selectedID using the useState hook, which keeps track of the ID of the selected flashcard.
Defines a handleClick function that toggles the selected flashcard's ID when clicked.

### Rendering Flashcards:

Utilizes the map function to iterate through the questions array and generate HTML elements for each flashcard.
Each flashcard div has an onClick event that triggers the handleClick function when clicked.
The key attribute ensures the uniqueness of each flashcard element.
The class name "selected" is conditionally applied to the selected flashcard based on selectedID.
Displays either the question or answer based on whether the flashcard is selected.
