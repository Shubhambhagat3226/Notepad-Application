# Shubhambhagat3226 Notepad Application

A simple Notepad application built with Java and Swing, offering essential text editing functionalities and a customizable user interface.

## Features

*   **File Management:**
    *   **New:** Create a blank document.
    *   **Open:** Open existing `.txt` files.
    *   **Save:** Save changes to the current file or prompt for a new file.
    *   **Save As:** Save the document to a new file with a custom name and location.
    *   **Exit:** Close the application.

*   **Editing:**
    *   **Undo:** Reverse the last action.
    *   **Redo:** Reapply the previously undone action.

*   **Formatting:**
    *   **Word Wrap:** Toggle text wrapping within the window.
    *   **Align Text:**  Align text to the left or right.
    *   **Font:** Customize font family, style (bold, italic), size, and color.

*   **View:**
    *   **Zoom:**
        *   **Zoom In:** Increase the font size.
        *   **Zoom Out:** Decrease the font size (minimum size 9).
        *   **Restore Default Zoom:** Reset the font size to 12.

*   **User Interface:** Enhanced with JTattoo's Acryl Look and Feel.

## Requirements

*   Java Development Kit (JDK) 8 or later.
*   JTattoo library (JTattoo-1.6.13.jar) - included in the `lib/` directory.

## Installation

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/Shubhambhagat3226/Notepad-Application.git
    cd notepad-application
    ```

2.  **Compile the code:**

    Using the command line:

    ```bash
    javac -cp "lib/JTattoo-1.6.13.jar:." src/*.java
    ```

    Alternatively, import the `Notepad App.iml` file into IntelliJ IDEA or another compatible IDE.  Ensure the JTattoo library is in the project's classpath.

3.  **Run the application:**

    ```bash
    java -cp "lib/JTattoo-1.6.13.jar:." App
    ```

## Project Structure

shubhambhagat3226-notepad-application/
├── Notepad App.iml
├── lib/
│   └── JTattoo-1.6.13.jar
├── src/
│   ├── App.java
│   ├── FontMenu.java
│   ├── NotepadGui.java
│   └── Assets/
│       ├── random.txt
│       └── text.txt
└── README.md


## How to Use

1.  Launch the application using the instructions above.
2.  Use the menu bar to access File, Edit, Format, and View options.
3.  Customize the font through the "Format" -> "Font..." menu.
4.  Adjust the zoom level with "View" -> "Zoom" options.

## Dependencies

*   **JTattoo:** Provides a polished user interface.  See [http://www.jtattoo.net/](http://www.jtattoo.net/) for more information.

## Important Notes

*   The application automatically appends `.txt` to saved files if no extension is provided.
*   The user interface theme can be modified in `App.java` by changing the `UIManager.setLookAndFeel` value.
*   The default directory for file operations is set to `src/Assets`.
