# c199

A threaded TCP quiz server that serves random multiple-choice questions and tracks scores.

## Features
- Socket server on `127.0.0.1:8000` accepting multiple clients
- Thread-per-client question/answer loop
- Random questions drawn from a small built-in question bank
- Live score tracking and correct/incorrect feedback
- Removes used questions so no question repeats per game

## Tech Stack
- Python 3, standard library (`socket`, `threading`, `random`)

## Project Structure
```
quiz_server.py     # server + quiz game logic
```

## Installation
No dependencies — Python 3 only.

## Usage
```
python quiz_server.py
```
Connect a client, e.g. `nc 127.0.0.1 8000`, and answer the questions with `a`/`b`/`c`/`d`.