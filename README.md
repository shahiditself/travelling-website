# travelling-website
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>WONDERTRAILS - Travel Agency</title>
    <style>
        * {margin: 0; padding: 0; box-sizing: border-box;}
        body {font-family: 'Segoe UI', sans-serif; line-height: 1.6; color: #333; background: linear-gradient(to bottom right, #f5f7fa, #c3cfe2);}
        header {background: linear-gradient(to right, #ff416c, #ff4b2b); color: #fff; padding: 20px; text-align: center;}
        nav ul {display: flex; justify-content: center; list-style: none; background: linear-gradient(to right, #00b4db, #0083b0);}
        nav ul li {margin: 0 15px;}
        nav ul li a {color: #fff; text-decoration: none; padding: 10px; display: block; font-weight: bold;}
        nav ul li a:hover {background: rgba(255,255,255,0.2); border-radius: 5px;}

        .slider {position: relative; overflow: hidden; height: 400px;}
        .slides {display: flex; animation: slide 16s infinite;}
        .slide {min-width: 100%; height: 400px; background-size: cover; background-position: center; display: flex; align-items: center; justify-content: center; color: #fff; font-size: 2.5rem; font-weight: bold; text-shadow: 2px 2px 4px #000;}

        @keyframes slide {
            0% {transform: translateX(0%);}
            25% {transform: translateX(-100%);}
            50% {transform: translateX(-200%);}
            75% {transform: translateX(-300%);}
            100% {transform: translateX(0%);}
        }

        section {padding: 50px 20px;}
        .destinations, .packages, .reviews, .owners, .booking, .group-booking {text-align: center;}

        h2 {color: #0d47a1; margin-bottom: 20px;}

        .card {
            background: linear-gradient(135deg, #f8ffae 0%, #43c6ac 100%);
            border-radius: 12px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
            margin: 20px;
            padding: 20px;
            display: inline-block;
            width: 250px;
            color: #333;
            transition: transform 0.3s;
        }
        .card:hover {transform: scale(1.05);}
        .card img {width: 100%; border-radius: 10px; height: 150px; object-fit: cover; margin-bottom: 10px;}

        .booking-form {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 10px;
            max-width: 400px;
            margin: 0 auto;
            background: #fff;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }
        .booking-form input, .booking-form select, .booking-form button {
            width: 100%; padding: 10px; border-radius: 5px; border: 1px solid #ccc;
        }
        .booking-form button {background: #ff416c; color: #fff; border: none; cursor: pointer; font-weight: bold;}
        .booking-form button:hover {background: #ff4b2b;}

        footer {
            background: linear-gradient(to right, #00c6ff, #0072ff);
            color: #fff;
            text-align: center;
            padding: 20px;
        }
    </style>
</head>
<body>
<header>
    <h1>WONDERTRAILS</h1>
    <p>Your Gateway to Adventure</p>
</header>

<nav>
    <ul>
        <li><a href="#destinations">Destinations</a></li>
        <li><a href="#packages">Packages</a></li>
        <li><a href="#reviews">Reviews</a></li>
        <li><a href="#owners">Owners</a></li>
        <li><a href="#booking">Booking</a></li>
        <li><a href="#group-booking">Group Trips</a></li>
    </ul>
</nav>

<div class="slider">
    <div class="slides">
        <div class="slide" style="background-image: url('https://source.unsplash.com/1600x900/?india,goa');">Relax in Goa</div>
        <div class="slide" style="background-image: url('https://source.unsplash.com/1600x900/?india,jaipur');">Explore Jaipur</div>
        <div class="slide" style="background-image: url('https://source.unsplash.com/1600x900/?india,kerala');">Kerala Backwaters</div>
        <div class="slide" style="background-image: url('https://source.unsplash.com/1600x900/?india,manali');">Adventures in Manali</div>
    </div>
</div>

<section id="destinations" class="destinations">
    <h2>Popular Destinations</h2>
    <div class="card"><img src="https://source.unsplash.com/300x200/?goa,beach" alt="Goa"><h3>Goa</h3><p>Sunny beaches and nightlife</p></div>
    <div class="card"><img src="https://source.unsplash.com/300x200/?jaipur,fort" alt="Jaipur"><h3>Jaipur</h3><p>Royal forts & palaces</p></div>
    <div class="card"><img src="https://source.unsplash.com/300x200/?kerala,backwater" alt="Kerala"><h3>Kerala</h3><p>Backwaters & greenery</p></div>
    <div class="card"><img src="https://source.unsplash.com/300x200/?manali,mountains" alt="Manali"><h3>Manali</h3><p>Snow-clad mountains</p></div>
</section>

<section id="packages" class="packages">
    <h2>Travel Packages</h2>
    <div class="card"><h3>Goa Special</h3><p>₹3,000 per person - 3 Nights</p></div>
    <div class="card"><h3>Jaipur Heritage</h3><p>₹4,500 per person - 4 Nights</p></div>
    <div class="card"><h3>Kerala Retreat</h3><p>₹6,000 per person - 5 Nights</p></div>
    <div class="card"><h3>Manali Adventure</h3><p>₹5,000 per person - 4 Nights</p></div>
</section>

<section id="reviews" class="reviews">
    <h2>Customer Reviews</h2>
    <div class="card"><h3>Rohit Sharma</h3><p>"Amazing service, booked my honeymoon to Kerala!"</p></div>
    <div class="card"><h3>Priya Sinha</h3><p>"Loved the Jaipur trip! Well organized and fun."</p></div>
    <div class="card"><h3>Amit Patel</h3><p>"Nomadic Trails made our Goa vacation unforgettable!"</p></div>
</section>

<section id="owners" class="owners">
    <h2>Meet the Owners</h2>
    <div class="card"><img src="https://via.placeholder.com/300x200?text=Upload+Photo" alt="Shahid Take"><h3>Shahid Take</h3><p>Founder & Travel Enthusiast</p></div>
    <div class="card"><img src="https://via.placeholder.com/300x200?text=Upload+Photo" alt="Nomam Khureshi"><h3>Nomam Khureshi</h3><p>Co-Founder & Operations Head</p></div>
</section>

<section id="booking" class="booking">
    <h2>Book Your Trip</h2>
    <form class="booking-form" onsubmit="alert('Booking Successful!'); return false;">
        <input type="text" placeholder="Full Name" required>
        <input type="email" placeholder="Email Address" required>
        <select required>
            <option value="">Select Destination</option>
            <option>Goa - ₹3,000</option>
            <option>Jaipur - ₹4,500</option>
            <option>Kerala - ₹6,000</option>
            <option>Manali - ₹5,000</option>
        </select>
        <button type="submit">Book Now</button>
    </form>
</section>

<section id="group-booking" class="group-booking">
    <h2>Group Trip Booking</h2>
    <form class="booking-form" onsubmit="alert('Group Booking Successful!'); return false;">
        <label for="group-destination">Destination</label>
        <select id="group-destination" required>
            <option value="">Select Destination</option>
            <option>Goa - ₹800 per person</option>
            <option>Jaipur - ₹1,200 per person</option>
            <option>Kerala - ₹2,000 per person</option>
            <option>Manali - ₹1,500 per person</option>
        </select>

        <label for="people">Number of People</label>
        <input type="number" id="people" min="2" max="20" required>

        <button type="submit">Book Group Trip</button>
    </form>
</section>

<footer>
    <p>© 2025 WONDERTRAILS. All rights reserved.</p>
</footer>

</body>
</html>
