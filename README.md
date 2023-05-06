# Harmony
This Python program is used to implement a music player using the Pygame library while browsing songs on one's computer. The program uses the PySide6. QtCore and PySide6. QtWidgets libraries for the graphical user interface.

GUI Elements
The GUI elements of the music player include:
•	A QListWidget for displaying the playlist
•	A QPushButton for playing the selected song
•	A QPushButton for stopping the current song
•	A QPushButton for looping the current song
•	A QPushButton for adding songs to the playlist
The QListWidget is limited to a maximum size of 400x300 pixels.
Functionality
The program uses the Pygame library for playing the music, and includes the following functions:
play()
This function plays the selected song from the playlist. If no song is selected, the user is notified with an information message. If a song is selected, the function stops the currently playing music, loads the selected song, and plays it from the beginning.
stop()
This function stops the currently playing music.
loop()
This function stops the currently playing music and starts playing it again from the beginning, in a loop.
add()
This function opens a file dialog window, allowing the user to select audio files to add to the playlist. The function supports files with extensions .mp3, .ogg, and .wav. The selected files are added to the playlist and displayed in the QListWidget.
closeEvent(event)
This function is called when the user attempts to close the application. It stops the currently playing music and quits the Pygame library before closing the application.
Pygame Initialization
The Pygame library is initialized at the start of the program.
Main Function
The main function creates a new instance of the Application class, which is a QWidget that contains the GUI elements for the music player. It then runs the application loop using app.exec_().
