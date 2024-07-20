# Gyst Chat Room Application

This is a simple chat room application built with Flask and Flask-SocketIO. It allows users to create and join chat rooms and send messages in real-time.

## Features

- Create a new chat room with a unique code
- Join an existing chat room using a code
- Send and receive messages in real-time
- Display notifications when users join or leave the room

## Requirements

- Python 3.x
- Flask
- Flask-SocketIO

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/Olutayo0910/Gyst.git
    cd Gyst
    ```

2. Create a virtual environment and activate it:

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. Install the required packages:

    ```bash
    pip install -r requirements.txt
    ```

## Configuration

Set the secret key for the Flask application. You can update the `SECRET_KEY` in the `app.config` section of `main.py`:

```python
app.config['SECRET_KEY'] = "your_secret_key"

## Running the Application
```bash
python main.py
```
The application will start running on http://127.0.0.1:5000.

## Usage

Open a web browser and navigate to http://127.0.0.1:5000.
Enter your name.
To create a new room, click "Create". A unique room code will be generated.
To join an existing room, enter the room code and click "Join".
Start chatting!

## Application Structure

main.py: The main application file containing routes and SocketIO event handlers.
templates/: Directory containing HTML templates (home.html and room.html).

## Routes

/: Home route where users can enter their name and create/join a room.
/room: Room route where users can chat.

## SocketIO Events

message: Handles incoming messages and broadcasts them to the room.
connect: Handles new connections to the room.
disconnect: Handles disconnections from the room.

## Contributing

Feel free to fork this repository, make improvements, and submit a pull request. Contributions are welcome!

