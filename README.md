# Keem Road House — interactive demo

Static, zero-dependency proof of concept for a two-room guesthouse on Achill Island. Built from the supplied property overview, requirements and photo archive.

## Start locally

Open `index.html` in a browser, or serve the folder using `python -m http.server 8080` and visit `http://localhost:8080`.

## Included

- Responsive branded home page, room photos, gallery, local attractions, directions and contact screen.
- Availability search with a **two-night minimum**, one or two room selection, individual room allocation and browser-local conflict checks.
- Default **€200 per room per night** with date/room-specific admin overrides.
- Guest details and demo checkout: **no card fields, no charges, no real reservations**.
- Cancellation terms shown before checkout: full refund before **10:00 am Ireland local time seven days prior**; 100% charge for later cancellation/change or no-show. The demo account page supports cancellation before the deadline.
- **3 pm check-in**, **12 noon check-out**.
- Local-only demo accounts and a dedicated **Enter admin demo** button on the login page; admin calendar, date blocks, price overrides, booking records and inspection confirmation.
- Real property photographs, converted to WebP to reduce download sizes.

## Explicitly not production-ready

The prototype stores bookings, prices, sample accounts and admin flag in browser localStorage, not in a server. **Do not use for real bookings or collect real customer credentials.** Data do not sync across devices or browsers. Login is simulated; sample passwords are stored insecurely in localStorage. No email is sent, and the contact form is illustrative. No Airbnb integration, payment processor, post-checkout charging, damage fee handling or review submissions are implemented.

Next: Supabase authentication and database (atomic room-night reservation protections and server-enforced authorisation), provider-hosted payment integration, email delivery, and safe Airbnb coexistence if needed.

All demo data are local to the browser and may be cleared via browser storage settings.
