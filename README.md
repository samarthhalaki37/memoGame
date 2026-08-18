# Flask Memory Game

A simple and interactive **Memory Game** built with **Flask**, HTML, CSS, and JavaScript. The goal is to match all pairs of cards using as few moves as possible.

## Features

* 🎮 Interactive memory card game
* 🔀 Cards are randomly shuffled for every game
* 🧠 Match pairs of identical cards
* 📊 Tracks the number of moves
* 🔄 Restart the game at any time
* 📱 Responsive and user-friendly interface
* ⚡ Lightweight Flask backend

## Technologies Used

* **Python 3**
* **Flask**
* **HTML5**
* **CSS3**
* **JavaScript**

## Project Structure

```text
flask-memory-game/
│
├── app.py                 # Flask application
├── requirements.txt       # Python dependencies
│
├── templates/
│   └── index.html         # Main game page
│
├── static/
│   ├── css/
│   │   └── style.css      # Game styling
│   │
│   └── js/
│       └── script.js      # Game logic
│
└── README.md              # Project documentation
```

## Getting Started

### 1. Clone the Repository

```bash
git clone <repository-url>
cd flask-memory-game
```

### 2. Create a Virtual Environment

```bash
python -m venv venv
```

Activate the virtual environment:

**Windows:**

```bash
venv\Scripts\activate
```

**Linux/macOS:**

```bash
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Application

```bash
python app.py
```

The application will start on the local Flask development server.

Open your browser and visit:

```text
http://127.0.0.1:5000/
```

## How to Play

1. Click on a card to reveal it.
2. Click on a second card.
3. If the two cards match, they remain visible.
4. If they do not match, they are hidden again.
5. Continue until all pairs have been matched.
6. Try to complete the game using the fewest possible moves.

## Flask Application

The Flask server is responsible for serving the main game page and static assets. The core game mechanics, including card flipping, matching, shuffling, and move tracking, are handled on the client side with JavaScript.

A basic Flask application can be structured like this:

```python
from flask import Flask, render_template

app = Flask(__name__)


@app.route("/")
def home():
    return render_template("index.html")


if __name__ == "__main__":
    app.run(debug=True)
```

## Requirements

Example `requirements.txt`:

```text
Flask
```

Install the requirements with:

```bash
pip install -r requirements.txt
```

## Future Improvements

Possible enhancements include:

* Add difficulty levels
* Add a timer
* Add a high-score system
* Store scores in a database
* Add sound effects
* Add animations
* Add multiple card themes
* Add user accounts and leaderboards

## License

This project is open-source and available for educational and personal use. Add an appropriate license file if you plan to distribute the project publicly.
