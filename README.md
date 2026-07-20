 ⏱️ PyQt5 Stopwatch

A modern stopwatch application built with Python and PyQt5 that allows users to start, stop, and reset a high-precision timer through a clean graphical user interface.



📌 Overview

The PyQt5 Stopwatch is a desktop application that measures elapsed time with centisecond precision.

The application features:

* Start functionality
* Stop functionality
* Reset functionality
* Real-time display updates
* Custom user interface styling

This project demonstrates how event-driven applications work using PyQt5 while introducing concepts such as timers, signals and slots, GUI layouts, and object-oriented programming.



Features

* High-precision stopwatch
* Start timer
* Stop timer
* Reset timer
* Real-time updates every 10 milliseconds
* Modern graphical interface
* Custom widget styling
* Responsive layouts



Technologies Used

* Python 3
* PyQt5



Installation

Install PyQt5

```bash
pip install PyQt5
```

Clone the Repository

```bash
git clone https://github.com/Abdurrahman-byte/pyqt5-stopwatch.git
```

Navigate to the Project Directory

```bash
cd pyqt5-stopwatch
```

Run the Application

```bash
python main.py
```



User Interface

The application contains:

| Component    | Purpose                  |
| ------------ | ------------------------ |
| Time Display | Shows elapsed time       |
| Start Button | Starts the stopwatch     |
| Stop Button  | Pauses the stopwatch     |
| Reset Button | Resets the timer to zero |



Project Structure

```text
pyqt5-stopwatch/
│
├── alarm.py
└── README.md
```



How to Use

Start the Stopwatch

Click:

```text
Start
```

The timer begins counting immediately.



Stop the Stopwatch

Click:

```text
Stop
```

The timer pauses while preserving the current elapsed time.



Reset the Stopwatch

Click:

```text
Reset
```

The timer returns to:

```text
00:00:00.00
```



Time Format

The stopwatch displays time in the following format:

```text
HH:MM:SS.CC
```

Where:

* HH = Hours
* MM = Minutes
* SS = Seconds
* CC = Centiseconds

Example:

```text
01:15:42.35
```

means:

* 1 hour
* 15 minutes
* 42 seconds
* 35 centiseconds



How It Works

QTimer

The application uses a PyQt5 `QTimer`.

```python
self.timer.start(10)
```

The timer triggers every:

```text
10 milliseconds
```



Updating Time

Each timer tick adds:

```python
self.time.addMSecs(10)
```

to the current stopwatch value.



Formatting Display

The time is converted into a readable format:

```text
HH:MM:SS.CC
```

before being displayed on screen.



Concepts Practiced

This project helped reinforce:

* Object-Oriented Programming (OOP)
* Classes and Methods
* GUI Development
* Event-Driven Programming
* Signals and Slots
* Timers
* Layout Management
* Widget Styling
* Time Manipulation
* Desktop Application Development



UI Features

Styled Buttons

The application uses custom stylesheets to create larger, more user-friendly controls.

Large Time Display

The stopwatch display uses:

```text
120px font size
```

for improved readability.

Rounded Interface

The timer display features rounded corners and a custom background color for a modern appearance.



Future Improvements

* Lap Timer Support
* Save Lap Records
* Export Times to File
* Dark Mode
* Alarm Notifications
* Keyboard Shortcuts
* Statistics Tracking
* Fullscreen Mode



Current Limitations

* No lap recording functionality
* No persistent storage
* Single stopwatch instance
* No keyboard controls



Author

Abdurrahman

Python Developer | Aspiring AI/ML Engineer



Project Goal

This project was built to explore desktop application development with PyQt5 while practicing object-oriented programming and event-driven design.

It demonstrates how timers, GUI components, layouts, and user interactions can be combined to create a responsive and professional desktop application.

The project serves as a strong introduction to building more advanced PyQt5 applications such as productivity tools, dashboards, timers, and utility software.
