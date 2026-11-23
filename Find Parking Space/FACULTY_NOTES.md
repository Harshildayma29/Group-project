# Faculty Explanation Notes – ParkEasy

## 40-second introduction
"My project is ParkEasy, a simple Smart Parking Finder website. The problem is that people spend time searching for parking, especially in crowded areas. My prototype shows sample Ahmedabad parking locations and displays separate bike and car parking spaces. It also supports basic registration, booking and cancellation. I used HTML, CSS and JavaScript for the website, Python built-in web server for the backend, and SQLite to store data. This is a local student prototype; it is not connected to real sensors or a payment gateway."

**Customize this wording to accurately describe your own work and contributions.**

## Demonstrate it in order
1. Open http://127.0.0.1:5000/ after running `python server.py`.
2. Search "Vastrapur" and change the vehicle type.
3. Show the separate spaces and per-hour price.
4. Register a demo account or log in.
5. Select Book Now, duration 2 hours, and confirm a demo booking.
6. Open My Bookings and show the reservation.
7. Run `python view_data.py` to show the booking in SQLite.
8. Cancel the booking and show the available slot count increasing again.

## Viva questions
**Q1. Why use SQLite?**
A: It saves data in a simple local file without needing a separate database server.

**Q2. What is the role of Python?**
A: It receives requests from the browser, reads and writes database records, and returns results.

**Q3. Where is HTML/CSS/JS used?**
A: HTML defines the page, CSS gives it style, and JavaScript loads parking cards and sends booking requests.

**Q4. How does the booking change availability?**
A: When a booking is saved, available spaces for that vehicle type decrease by one. Cancellation increases them by one.

**Q5. Is it a real-time system?**
A: No. The website displays demonstration data updated by demo bookings, not information from actual parking sensors.

**Q6. Is it an ML prediction system?**
A: No. The estimate is calculated with `available / total * 100`, a basic percentage.

**Q7. Does payment really happen?**
A: No. The payment page is a classroom demonstration and does not collect money.

**Q8. What is the design thinking process?**
A: Empathize, Define, Ideate, Prototype and Test. See DESIGN_THINKING.md.

## Improvements you can implement yourself
- Add a new local parking location using add_parking.py
- Change the project colors in static/style.css
- Interview 3–5 drivers and record their feedback
- Add screenshots of your own working website to the project report

Only describe work you actually completed and understand.

## Added Ahmedabad areas
The updated demo uses 48 illustrative parking locations across Ahmedabad, with
separate two-wheeler/four-wheeler spaces and simple area filtering.
Explain clearly that these are illustrative records stored in SQLite, not live parking sensors.
