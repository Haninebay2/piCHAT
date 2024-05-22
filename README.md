
# PieChat

PieChat is a simple yet robust chat application built with Python that enables users to communicate over a network. The project includes two main parts: a graphical user interface (GUI) using Tkinter for interactive use, and a command-line interface (CLI) that manages network functionalities using both TCP and UDP protocols.

## Features

- **User Authentication**: Users can log in with predefined credentials.
- **Contact List**: Displays a list of available contacts for communication.
- **Messaging**: Supports sending and receiving text messages in real-time using UDP.
- **File Transfer**: Allows users to send and receive files using TCP.
- **Error Handling**: Includes basic error handling for network issues and user authentication.

## Installation

To run PieChat, you need Python installed on your system. Python 3.6 or higher is recommended. You can download Python from [python.org](https://www.python.org/downloads/).

### Dependencies

Before running the application, install the necessary dependencies:

```bash
pip install tkinter
```

## Usage

The project is split into two parts: the GUI application (`gui.py`) and the command-line network functionality (`network.py`). Here’s how to use each:

### GUI Application

1. Navigate to the directory containing `gui.py`.
2. Run the following command:

```bash
python gui.py
```

This starts the GUI version of PieChat, where users can log in, select a contact, and start chatting or sending files.

### Network Functionality

1. Navigate to the directory containing `network.py`.
2. Run the following command:

```bash
python network.py
```

This starts the CLI version of PieChat, managing the sending/receiving of messages and files through command-line inputs.

## Network Details

- **UDP (User Datagram Protocol)**: Used for sending messages between users. UDP is a connectionless protocol, which means it sends data without establishing a connection, thus making it faster but less reliable.
- **TCP (Transmission Control Protocol)**: Used for file transfer functionality. Unlike UDP, TCP is connection-oriented and ensures that data is delivered accurately and in sequence.
- **IP Address Conversion**: Converts IP addresses to integer format for easier manipulation and checksum calculations in networking operations.
- **Checksum Functionality**: Implements a checksum for validating message integrity during transmissions. This helps detect errors or alterations in the data.
- **Error Handling**: Provides basic mechanisms to handle errors such as network disconnections, unavailable services, or transmission errors.

## Configuration

The application uses hardcoded user and contact details for simplicity. These can be found and modified in the `contacts` dictionary within both script files.

## Contributing

Contributions to PieChat are welcome. Please ensure to follow the existing coding style and add comments where necessary. Create a pull request with a description of your changes or improvements.
