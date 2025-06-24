No-Database Emergency Response System

Files:
- user.html: Used to send an emergency alert (with case and GPS location).
- admin.html: Receives and displays alerts in real-time (same browser/device).

How It Works:
- Uses BroadcastChannel API (works when both pages are open in same browser).
- Gets user's location and address using Geolocation + OpenStreetMap.
- Plays loud siren (user) and bell (admin) on each alert.

Note:
- No data is saved permanently (only in memory).
- Works best on the same device/browser (can’t communicate across devices without a server).
