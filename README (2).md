# TomatoSetu (టమాటో సేతు)

Telugu-first voice prototype that matches small tomato farmers around Kakinada, Andhra Pradesh with nearby buyers on the same day.

**All buyers, prices and distances are demo data, not live market information.** No API keys or secrets are used.

## Run with one command
```
docker compose up --build
```
Open http://localhost:8080 in Chrome (microphone works on localhost).

Without Docker, open `index.html` in Chrome, or run `python -m http.server 8080` in this folder.

## Try it
- Tap **Try sample farmer** to play the full flow without speaking.
- Tap the microphone and speak Telugu, for example: "Naa daggara 200 kilolu tomatoes unnayi, ee roje ammali".
- Or type in the text box and use the Yes/No and chip buttons.

## Notes
- Uses the browser's Web Speech API (te-IN). Needs Chrome and an internet connection. Telugu voice output needs a Telugu voice installed on the device; otherwise captions are shown.
- If the microphone is blocked or speech is unclear, the app falls back to buttons and typing.
- Matching uses quantity, distance, price and same-day availability.
