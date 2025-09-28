# vahan bazar
project is a bikes selling website vahanbazar
index.html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Two-Wheeler Marketplace</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>
    <!-- Header Section -->
    <header class="header">
        <div class="logo">BikeBazaar</div>

        <!-- Navigation -->
        <nav class="nav">
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">Browse</a></li>
                <li><a href="#">Compare</a></li>
                <li><a href="#">Showrooms</a></li>
                <li><a href="#">Sell Bike</a></li>
                <li><a href="#">Contact</a></li>
            </ul>
        </nav>

        <!-- Right Actions -->
        <div class="actions">
            <i class="fas fa-search"></i>
            <button class="login-btn">Login / Signup</button>
            <i class="fas fa-bars menu-toggle"></i>
        </div>
    </header>
    <!-- Hero Section -->
    <section class="hero">
        <h1>Find Your Perfect Ride</h1>
        <p>Browse, compare, and book bikes, scooters, and EVs — all in one place.</p>
        <div class="btn-group">
            <button class="btn btn-primary">Browse Bikes</button>
            <button class="btn btn-secondary">Sell Your Bike</button>
        </div>
    </section>
    <!-- Search & Filter Quick Bar -->
    <section class="search-bar">
        <form>
            <input type="text" placeholder="Search by model or brand">

            <select>
        <option value="">Select Type</option>
        <option value="bike">Bike</option>
        <option value="scooter">Scooter</option>
        <option value="ev">EV</option>
      </select>

            <select>
        <option value="">Fuel Type</option>
        <option value="petrol">Petrol</option>
        <option value="electric">Electric</option>
        <option value="hybrid">Hybrid</option>
      </select>

            <input type="number" placeholder="Max Price (₹)">

            <button type="submit" class="btn-search">🔍 Search</button>
        </form>
    </section>
    <!-- Featured Bikes / Trending Now -->
    <section class="featured">
        <h2>🔥 Featured Bikes / Trending Now</h2>
        <div class="bike-grid">

            <div class="bike-card">
                <img src="https://imgd.aeplcdn.com/370x208/n/cw/ec/108277/yamaha-yzf-r15-right-side-view1.jpeg?isig=0&q=80" alt="Bike 1">
                <h3>Yamaha R15 V4</h3>
                <p>Price: ₹1,80,000</p>
                <button>View Details</button>
            </div>

            <div class="bike-card">
                <img src=" https://imgd.aeplcdn.com/664x374/n/cw/ec/183389/classic-350-right-front-three-quarter-2.jpeg?isig=0&q=80" alt="Bike 2">
                <h3>Royal Enfield Classic 350</h3>
                <p>Price: ₹2,10,000</p>
                <button>View Details</button>
            </div>

            <div class="bike-card">
                <img src=" https://cdn.bikedekho.com/processedimages/ather-energy/2025-450x/source/2025-450x68a6c30d69e5f.jpg?imwidth=412&impolicy=resize" alt="Bike 3">
                <h3>Ather 450X EV</h3>
                <p>Price: ₹1,40,000</p>
                <button>View Details</button>
            </div>

            <div class="bike-card">
                <img src="https://imgd.aeplcdn.com/1056x594/n/rmpdpgb_1854140.jpg?q=80" alt="Bike 4">
                <h3>Honda Activa 6G</h3>
                <p>Price: ₹75,000</p>
                <button>View Details</button>
            </div>

        </div>
    </section>
    <!-- Comparison Teaser Section -->
    <section class="comparison">
        <h2>⚡ Compare Before You Decide</h2>
        <p class="subtitle">Check specs, features, and pricing side by side.</p>

        <div class="comparison-grid">

            <!-- Bike 1 -->
            <div class="compare-card">
                <img src="https://images.unsplash.com/photo-1605714224887-03c1b5965ec1" alt="Yamaha R15">
                <h3>Yamaha R15 V4</h3>
                <ul>
                    <li>💰 ₹1,80,000</li>
                    <li>⛽ Petrol</li>
                    <li>🏍️ 155cc Engine</li>
                    <li>📈 45 km/l</li>
                </ul>
            </div>

            <!-- VS Column -->
            <div class="vs-box">
                <span>VS</span>
            </div>

            <!-- Bike 2 -->
            <div class="compare-card">
                <img src="https://images.unsplash.com/photo-1617814076904-198d2fd4b50b" alt="Ather 450X EV">
                <h3>Ather 450X EV</h3>
                <ul>
                    <li>💰 ₹1,40,000</li>
                    <li>🔋 Electric</li>
                    <li>⚡ 6kW Motor</li>
                    <li>📈 146 km/charge</li>
                </ul>
            </div>

        </div>

        <button class="btn-compare">🔍 Compare Models →</button>
    </section>
    <!DOCTYPE html>
    <html lang="en">

    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Tools Section</title>
        <link rel="stylesheet" href="style.css">
    </head>

    <body>

        <!-- Tools Section -->
        <section class="tools">
            <h2>🛠️ Tools & Calculators</h2>
            <p class="subtitle">Plan your purchase smartly with our quick calculators.</p>

            <div class="tools-grid">

                <!-- EMI Calculator -->
                <div class="tool-card">
                    <h3>💳 EMI Calculator</h3>
                    <label>Loan Amount (₹)</label>
                    <input type="number" id="loan" placeholder="e.g. 100000">

                    <label>Interest Rate (%)</label>
                    <input type="number" id="rate" placeholder="e.g. 8">

                    <label>Tenure (months)</label>
                    <input type="number" id="months" placeholder="e.g. 24">

                    <button onclick="calculateEMI()">Calculate EMI</button>
                    <p class="result" id="emiResult">Your EMI will appear here</p>
                </div>

                <!-- Fuel Cost Calculator -->
                <div class="tool-card">
                    <h3>⛽ Fuel Cost Calculator</h3>
                    <label>Distance (km)</label>
                    <input type="number" id="distance" placeholder="e.g. 500">

                    <label>Mileage (km/l)</label>
                    <input type="number" id="mileage" placeholder="e.g. 40">

                    <label>Fuel Price (₹/l)</label>
                    <input type="number" id="fuelPrice" placeholder="e.g. 100">

                    <button onclick="calculateFuel()">Calculate Cost</button>
                    <p class="result" id="fuelResult">Fuel cost will appear here</p>
                </div>

            </div>
        </section>

        <script>
            function calculateEMI() {
                let loan = document.getElementById("loan").value;
                let rate = document.getElementById("rate").value;
                let months = document.getElementById("months").value;

                if (loan && rate && months) {
                    let monthlyRate = rate / 100 / 12;
                    let emi = (loan * monthlyRate * Math.pow(1 + monthlyRate, months)) /
                        (Math.pow(1 + monthlyRate, months) - 1);
                    document.getElementById("emiResult").innerText = "Monthly EMI: ₹" + emi.toFixed(2);
                } else {
                    document.getElementById("emiResult").innerText = "Please fill all fields.";
                }
            }

            function calculateFuel() {
                let distance = document.getElementById("distance").value;
                let mileage = document.getElementById("mileage").value;
                let fuelPrice = document.getElementById("fuelPrice").value;

                if (distance && mileage && fuelPrice) {
                    let cost = (distance / mileage) * fuelPrice;
                    document.getElementById("fuelResult").innerText = "Fuel Cost: ₹" + cost.toFixed(2);
                } else {
                    document.getElementById("fuelResult").innerText = "Please fill all fields.";
                }
            }
        </script>
        <!-- Upcoming Launches Section -->
        <section class="launches">
            <h2>🚀 Upcoming Launches</h2>
            <p class="subtitle">Stay ahead! Explore the latest two-wheelers arriving soon.</p>

            <div class="launches-grid">

                <!-- Card 1 -->
                <div class="launch-card">
                    <img src="https://via.placeholder.com/400x220" alt="Upcoming Bike">
                    <div class="launch-info">
                        <h3>Yamaha X500</h3>
                        <p class="date">Launching: Nov 2025</p>
                        <p class="specs">500cc • Petrol • ₹4.5L (Expected)</p>
                        <button>Notify Me</button>
                    </div>
                </div>

                <!-- Card 2 -->
                <div class="launch-card">
                    <img src="https://via.placeholder.com/400x220" alt="Upcoming Scooter">
                    <div class="launch-info">
                        <h3>Honda EV S1</h3>
                        <p class="date">Launching: Dec 2025</p>
                        <p class="specs">Electric • Range 180km • ₹1.2L (Expected)</p>
                        <button>Notify Me</button>
                    </div>
                </div>

                <!-- Card 3 -->
                <div class="launch-card">
                    <img src="https://via.placeholder.com/400x220" alt="Upcoming Bike">
                    <div class="launch-info">
                        <h3>Royal Enfield 650 Cruiser</h3>
                        <p class="date">Launching: Jan 2026</p>
                        <p class="specs">650cc • Petrol • ₹3.8L (Expected)</p>
                        <button>Notify Me</button>
                    </div>
                </div>

            </div>
        </section>
        <!-- Explore Showrooms Section -->
        <section class="showrooms">
            <h2>🏍️ Explore Showrooms</h2>
            <p class="subtitle">Find authorized showrooms near you to book test rides or explore two-wheelers in person.</p>

            <div class="showroom-grid">

                <!-- Showroom 1 -->
                <div class="showroom-card">
                    <h3>Bangalore Yamaha Center</h3>
                    <p class="city">📍 Bangalore, Karnataka</p>
                    <p class="address">12th Cross, MG Road, Bangalore - 560001</p>
                    <p class="contact">📞 +91 98765 43210</p>
                    <button>View on Map</button>
                </div>

                <!-- Showroom 2 -->
                <div class="showroom-card">
                    <h3>Honda EV Hub</h3>
                    <p class="city">📍 Hyderabad, Telangana</p>
                    <p class="address">Plot No 24, Hitech City, Hyderabad - 500081</p>
                    <p class="contact">📞 +91 99887 66554</p>
                    <button>View on Map</button>
                </div>

                <!-- Showroom 3 -->
                <div class="showroom-card">
                    <h3>Royal Enfield Exclusive</h3>
                    <p class="city">📍 Pune, Maharashtra</p>
                    <p class="address">FC Road, Shivaji Nagar, Pune - 411005</p>
                    <p class="contact">📞 +91 91234 56789</p>
                    <button>View on Map</button>
                </div>

            </div>
        </section>
        <!-- Test Ride Booking Section -->
        <section class="test-ride">
            <h2>🏍️ Book a Test Ride</h2>
            <p class="subtitle">Experience your dream two-wheeler before you buy. Fill in the details to book a test ride.</p>

            <form class="test-ride-form">
                <div class="form-group">
                    <label for="name">Full Name</label>
                    <input type="text" id="name" placeholder="Enter your full name">
                </div>

                <div class="form-group">
                    <label for="mobile">Mobile Number</label>
                    <input type="tel" id="mobile" placeholder="Enter your mobile number">
                </div>

                <div class="form-group">
                    <label for="vehicle">Select Vehicle</label>
                    <select id="vehicle">
          <option value="">Choose Vehicle</option>
          <option value="bike">Yamaha R15</option>
          <option value="scooter">Honda Activa</option>
          <option value="ev">Ather 450X</option>
          <option value="royal">Royal Enfield Classic</option>
        </select>
                </div>

                <div class="form-group">
                    <label for="date">Preferred Date</label>
                    <input type="date" id="date">
                </div>

                <div class="form-group">
                    <label for="time">Preferred Time</label>
                    <input type="time" id="time">
                </div>

                <div class="form-group">
                    <label for="showroom">Select Showroom</label>
                    <select id="showroom">
          <option value="">Choose Showroom</option>
          <option value="bangalore">Bangalore Yamaha Center</option>
          <option value="hyderabad">Honda EV Hub, Hyderabad</option>
          <option value="pune">Royal Enfield Exclusive, Pune</option>
        </select>
                </div>

                <button type="submit">Book Test Ride</button>
            </form>
        </section>
        <!-- Sell Your Bike Section -->
        <section class="sell-bike">
            <h2>💸 Sell Your Bike</h2>
            <p class="subtitle">Get the best price for your two-wheeler by listing it with us.</p>

            <form class="sell-bike-form">
                <!-- Owner Name -->
                <div class="form-group">
                    <label for="owner">Owner Name</label>
                    <input type="text" id="owner" placeholder="Enter your full name">
                </div>

                <!-- Mobile Number -->
                <div class="form-group">
                    <label for="mobile">Mobile Number</label>
                    <input type="tel" id="mobile" placeholder="Enter your mobile number">
                </div>

                <!-- Bike Brand & Model -->
                <div class="form-group">
                    <label for="bike">Bike Brand & Model</label>
                    <input type="text" id="bike" placeholder="e.g. Honda Activa 125">
                </div>

                <!-- Year of Purchase -->
                <div class="form-group">
                    <label for="year">Year of Purchase</label>
                    <input type="number" id="year" placeholder="e.g. 2020">
                </div>

                <!-- Expected Price -->
                <div class="form-group">
                    <label for="price">Expected Price (₹)</label>
                    <input type="number" id="price" placeholder="e.g. 65000">
                </div>

                <!-- Upload Image -->
                <div class="form-group">
                    <label for="photo">Upload Bike Photo</label>
                    <input type="file" id="photo" accept="image/*">
                </div>

                <!-- City -->
                <div class="form-group">
                    <label for="city">City</label>
                    <select id="city">
          <option value="">Select City</option>
          <option value="bangalore">Bangalore</option>
          <option value="hyderabad">Hyderabad</option>
          <option value="pune">Pune</option>
          <option value="delhi">Delhi</option>
        </select>
                </div>

                <!-- Submit -->
                <button type="submit">List My Bike</button>
            </form>
        </section>

        <!-- Testimonials Section -->
        <section class="testimonials">
            <h2>⭐ Customer Reviews</h2>
            <p class="subtitle">Hear what our happy riders have to say!</p>

            <div class="reviews">
                <!-- Review 1 -->
                <div class="review-card">
                    <img src="https://i.pravatar.cc/100?img=1" alt="User 1" class="avatar">
                    <h3>Rahul Verma</h3>
                    <p class="role">Bangalore</p>
                    <div class="stars">★★★★★</div>
                    <p class="review-text">"Smooth buying experience! I compared multiple bikes, booked a test ride, and purchased my dream bike easily. Highly recommended!"</p>
                </div>

                <!-- Review 2 -->
                <div class="review-card">
                    <img src="https://i.pravatar.cc/100?img=2" alt="User 2" class="avatar">
                    <h3>Ananya Sharma</h3>
                    <p class="role">Hyderabad</p>
                    <div class="stars">★★★★☆</div>
                    <p class="review-text">"The EMI calculator helped me plan my budget perfectly. The showroom locator was very handy too."</p>
                </div>

                <!-- Review 3 -->
                <div class="review-card">
                    <img src="https://i.pravatar.cc/100?img=3" alt="User 3" class="avatar">
                    <h3>Vikram Singh</h3>
                    <p class="role">Delhi</p>
                    <div class="stars">★★★★★</div>
                    <p class="review-text">"Sold my old scooter in just a few days. The process was seamless and transparent!"</p>
                </div>
            </div>
        </section>
        <!-- Footer -->
        <footer class="footer">
            <div class="footer-container">

                <!-- About -->
                <div class="footer-section about">
                    <h3>BikeBazaar</h3>
                    <p>Your one-stop marketplace for bikes, scooters, and EVs. Explore, compare, book test rides, and sell your two-wheelers with ease.</p>
                </div>

                <!-- Quick Links -->
                <div class="footer-section links">
                    <h4>Quick Links</h4>
                    <ul>
                        <li><a href="#">Browse Bikes</a></li>
                        <li><a href="#">Upcoming Launches</a></li>
                        <li><a href="#">Showrooms</a></li>
                        <li><a href="#">Sell Your Bike</a></li>
                        <li><a href="#">Contact Us</a></li>
                    </ul>
                </div>

                <!-- Contact -->
                <div class="footer-section contact">
                    <h4>Contact Us</h4>
                    <p><i class="fas fa-map-marker-alt"></i> Bangalore, India</p>
                    <p><i class="fas fa-phone"></i> +91 98765 43210</p>
                    <p><i class="fas fa-envelope"></i> support@bikebazaar.com</p>
                </div>

                <!-- Social -->
                <div class="footer-section social">
                    <h4>Follow Us</h4>
                    <div class="social-icons">
                        <a href="#"><i class="fab fa-facebook"></i></a>
                        <a href="#"><i class="fab fa-twitter"></i></a>
                        <a href="#"><i class="fab fa-instagram"></i></a>
                        <a href="#"><i class="fab fa-linkedin"></i></a>
                    </div>
                </div>

            </div>

            <!-- Bottom -->
            <div class="footer-bottom">
                <p>© 2025 BikeBazaar. All Rights Reserved.</p>
            </div>
        </footer>



    </body>

    </html>
