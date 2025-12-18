# Kanye Quote Generator

Small Python GUI app that fetches random quotes from the Kanye REST API and displays them in a styled window.

## Main features

- Tkinter window titled **"Kanye Says..."** with padding for a cleaner layout.
- Background image loaded from `background.png` and drawn on a `Canvas`.
- Quote text rendered in the centre of the window with custom font, width and colour.
- Button with `kanye.png` image; each click fetches a new quote.
- Uses the public API `https://api.kanye.rest` and updates the quote text live.

## What I learned

- Building graphical interfaces with Tkinter (window, canvas, images, buttons, layout).
- Loading and displaying PNG images using `PhotoImage`.
- Positioning widgets with the `grid` geometry manager.
- Making HTTP requests using the `requests` library.
- Working with JSON responses and updating existing UI elements via `canvas.itemconfig`.

## Project structure

- `main.py` – main script containing the Tkinter app and API integration.
- `background.png` – background image drawn behind the quote.
- `kanye.png` – image used on the button that triggers fetching a new quote.

## How to run

1. Make sure you have Python 3 installed.
2. Install the `requests` package with:

   `pip install requests`

3. Place `main.py`, `background.png` and `kanye.png` in the same folder.
4. From that folder, run:

   `python main.py`

A window titled **“Kanye Says…”** will open. Each time you click the Kanye button, the app calls the Kanye REST API and replaces the placeholder text with a new random quote.
