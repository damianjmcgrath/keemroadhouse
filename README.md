# Keem Road House

Interactive demo website for Keem Road House, Achill Island, County Mayo.

## Demo v0.1

The initial demo has been assembled as a ZIP in the associated ChatGPT conversation, but **the site files have not yet been pushed to this repository**.

The demo includes the property photographs, homepage, date availability search, one/two-room reservations, guest checkout simulation, gallery, directions, local area pages, and admin calendar.

### Demo assumptions
- €200 per room per night
- Two rooms; minimum two-night stay
- Check-in 3:00 pm; checkout noon
- Free cancellation before 10:00 am Irish local time seven days before arrival
- 100% cancellation fee after that cutoff or for no-shows
- No live payments, external bookings or Airbnb synchronization

### Publishing the demo from the downloaded ZIP

Extract the ZIP, open a terminal in the folder containing `index.html`, `app.js`, `style.css`, `README.md`, and `assets/`, then run:

```sh
git clone https://github.com/damianjmcgrath/keemroadhouse.git
# Copy all extracted demo files into the new keemroadhouse directory, including assets/
cd keemroadhouse
git add .
git commit -m "Add initial interactive Keem Road House demo"
git push origin main
```

Do not use this demo for real bookings. Its account and booking data are stored only in the local browser, and payment is simulated.
