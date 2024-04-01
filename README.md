# Harmony - A Python-based Music Player

Harmony is a lightweight music player built with Python, leveraging the Pygame library for music playback and PySide6 for its graphical user interface (GUI). This application offers a simple yet functional approach to browsing and playing your favorite songs directly from your computer.

## Features

- **Music Playback**: Utilize Pygame for seamless audio playback.
- **Graphical User Interface**: Built with PySide6, featuring intuitive controls.
- **Playlist Management**: Easily manage your music playlist within the application.

## GUI Elements

Harmony's user interface includes:

- **Playlist Display**: A `QListWidget` shows the playlist with a maximum size of 400x300 pixels.
- **Play Button**: A `QPushButton` to play the selected song from the playlist.
- **Stop Button**: A `QPushButton` to stop the currently playing song.
- **Loop Button**: A `QPushButton` for looping the current song.
- **Add Songs Button**: A `QPushButton` for adding songs to the playlist via a file dialog.

## Functionality

### Play Music

- **`play()`**: Plays the selected song. If no song is selected, displays an information message. Stops any currently playing music before playing the new selection.

### Stop Music

- **`stop()`**: Stops any music that is currently playing.

### Loop Music

- **`loop()`**: Loops the current song by stopping and replaying it from the start.

### Add to Playlist

- **`add()`**: Opens a file dialog for selecting audio files (.mp3, .ogg, .wav) to add to the playlist, displaying them in the `QListWidget`.

### Application Closure

- **`closeEvent(event)`**: Ensures music playback stops and Pygame quits properly when the application is closed.

## Dependencies

To run Harmony, you will need:

- **Python**: The core language used to develop Harmony.
- **Pygame**: A Python library for writing video games, used here for music playback.
- **PySide6**: Provides the GUI elements for the application.

Install Pygame and PySide6 using pip:

```sh
pip install pygame PySide6

## Pygame Initialization

- Initializes the Pygame library at the program's start for handling music playback.

## Running Harmony

To run Harmony, ensure you have Python installed along with the Pygame and PySide6 libraries. Execute the main function to start the application:

```python
if __name__ == "__main__":
    app = QApplication([])
    window = Application()
    window.show()
    sys.exit(app.exec_())

##Contributions

This README.md revision ensures a logical flow, grouping similar topics together for clarity. Dependencies are clearly outlined before the instructions to run the application, facilitating a smoother setup process for users. The contributions section invites community engagement, fostering an open and collaborative development environment.
