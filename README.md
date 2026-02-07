# Prabhat-s-Driving-School
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Special Driving School in Kolkata - Learn driving with confidence from experienced instructor Prabhat Ganguli. Affordable packages, safe teaching methods.">
    <title>Special Driving School - Learn Driving in Kolkata | Prabhat Ganguli</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --primary-blue: #2563eb;
            --dark-blue: #1e40af;
            --light-blue: #dbeafe;
            --dark-grey: #1f2937;
            --medium-grey: #6b7280;
            --light-grey: #f3f4f6;
            --white: #ffffff;
            --success-green: #10b981;
            --orange-accent: #f59e0b;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
            line-height: 1.6;
            color: var(--dark-grey);
            overflow-x: hidden;
        }

        /* Header & Navigation */
        header {
            background: var(--white);
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        nav {
            max-width: 1200px;
            margin: 0 auto;
            padding: 1rem 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--primary-blue);
        }

        .nav-links {
            display: flex;
            gap: 2rem;
            list-style: none;
        }

        .nav-links a {
            color: var(--dark-grey);
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
        }

        .nav-links a:hover {
            color: var(--primary-blue);
        }

        .mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            font-size: 1.5rem;
            cursor: pointer;
            color: var(--dark-grey);
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, var(--primary-blue) 0%, var(--dark-blue) 100%);
            color: var(--white);
            padding: 5rem 2rem;
            text-align: center;
        }

        .hero-content {
            max-width: 800px;
            margin: 0 auto;
        }

        .hero h1 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
            line-height: 1.2;
        }

        .hero p {
            font-size: 1.2rem;
            margin-bottom: 2rem;
            opacity: 0.95;
        }

        .cta-buttons {
            display: flex;
            gap: 1rem;
            justify-content: center;
            flex-wrap: wrap;
        }

        .btn {
            padding: 0.875rem 2rem;
            border: none;
            border-radius: 8px;
            font-size: 1rem;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s;
            text-decoration: none;
            display: inline-block;
        }

        .btn-primary {
            background: var(--white);
            color: var(--primary-blue);
        }

        .btn-primary:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 20px rgba(0,0,0,0.2);
        }

        .btn-secondary {
            background: transparent;
            color: var(--white);
            border: 2px solid var(--white);
        }

        .btn-secondary:hover {
            background: var(--white);
            color: var(--primary-blue);
        }

        /* Section Styling */
        section {
            padding: 4rem 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        .section-title {
            font-size: 2rem;
            text-align: center;
            margin-bottom: 3rem;
            color: var(--dark-grey);
        }

        .section-title::after {
            content: '';
            display: block;
            width: 60px;
            height: 4px;
            background: var(--primary-blue);
            margin: 1rem auto;
            border-radius: 2px;
        }

        /* About Section */
        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3rem;
            align-items: center;
        }

        .instructor-card {
            background: var(--light-grey);
            padding: 2rem;
            border-radius: 12px;
            text-align: center;
        }

        .instructor-card h3 {
            color: var(--primary-blue);
            font-size: 1.5rem;
            margin-bottom: 0.5rem;
        }

        .instructor-card p {
            color: var(--medium-grey);
            margin-bottom: 1rem;
        }

        /* Services Grid */
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 2rem;
        }

        .service-card {
            background: var(--white);
            padding: 2rem;
            border-radius: 12px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.08);
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .service-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 25px rgba(0,0,0,0.15);
        }

        .service-icon {
            font-size: 2.5rem;
            margin-bottom: 1rem;
        }

        .service-card h3 {
            color: var(--primary-blue);
            margin-bottom: 1rem;
        }

        /* Why Choose Us */
        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }

        .feature-item {
            text-align: center;
            padding: 1.5rem;
        }

        .feature-icon {
            width: 70px;
            height: 70px;
            background: var(--light-blue);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 1rem;
            font-size: 2rem;
        }

        .feature-item h3 {
            color: var(--dark-grey);
            margin-bottom: 0.5rem;
        }

        /* Pricing Section */
        .pricing-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 2rem;
        }

        .pricing-card {
            background: var(--white);
            border: 2px solid var(--light-grey);
            border-radius: 12px;
            padding: 2rem;
            text-align: center;
            transition: all 0.3s;
        }

        .pricing-card:hover {
            border-color: var(--primary-blue);
            transform: translateY(-5px);
        }

        .pricing-card.featured {
            border-color: var(--primary-blue);
            background: linear-gradient(135deg, var(--light-blue) 0%, var(--white) 100%);
        }

        .price-tag {
            font-size: 2.5rem;
            font-weight: 700;
            color: var(--primary-blue);
            margin: 1rem 0;
        }

        .price-features {
            list-style: none;
            margin: 1.5rem 0;
            text-align: left;
        }

        .price-features li {
            padding: 0.5rem 0;
            border-bottom: 1px solid var(--light-grey);
        }

        .price-features li:before {
            content: "✓ ";
            color: var(--success-green);
            font-weight: bold;
        }

        /* Signup Form */
        .signup-form {
            max-width: 600px;
            margin: 0 auto;
            background: var(--white);
            padding: 2rem;
            border-radius: 12px;
            box-shadow: 0 4px 20px rgba(0,0,0,0.1);
        }

        .form-group {
            margin-bottom: 1.5rem;
        }

        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 600;
            color: var(--dark-grey);
        }

        .form-group input,
        .form-group select,
        .form-group textarea {
            width: 100%;
            padding: 0.875rem;
            border: 2px solid var(--light-grey);
            border-radius: 8px;
            font-size: 1rem;
            transition: border-color 0.3s;
        }

        .form-group input:focus,
        .form-group select:focus,
        .form-group textarea:focus {
            outline: none;
            border-color: var(--primary-blue);
        }

        .payment-info {
            background: var(--light-blue);
            padding: 1.5rem;
            border-radius: 8px;
            margin: 1.5rem 0;
            text-align: center;
        }

        .payment-info h4 {
            color: var(--primary-blue);
            margin-bottom: 0.5rem;
        }

        .upi-id {
            font-size: 1.2rem;
            font-weight: 700;
            color: var(--dark-grey);
            background: var(--white);
            padding: 0.75rem;
            border-radius: 6px;
            margin-top: 0.5rem;
            display: inline-block;
        }

        /* Contact Section */
        .contact-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3rem;
        }

        .contact-info {
            background: var(--light-grey);
            padding: 2rem;
            border-radius: 12px;
        }

        .contact-item {
            display: flex;
            align-items: center;
            margin-bottom: 1.5rem;
            gap: 1rem;
        }

        .contact-icon {
            width: 50px;
            height: 50px;
            background: var(--primary-blue);
            color: var(--white);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5rem;
        }

        .map-container {
            width: 100%;
            height: 300px;
            border-radius: 12px;
            overflow: hidden;
            margin-top: 2rem;
        }

        /* Testimonials */
        .testimonials-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .testimonial-card {
            background: var(--white);
            padding: 2rem;
            border-radius: 12px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.08);
        }

        .testimonial-text {
            font-style: italic;
            color: var(--medium-grey);
            margin-bottom: 1rem;
        }

        .testimonial-author {
            font-weight: 600;
            color: var(--primary-blue);
        }

        .stars {
            color: var(--orange-accent);
            margin-bottom: 0.5rem;
        }

        /* Floating Action Buttons */
        .floating-btns {
            position: fixed;
            bottom: 2rem;
            right: 2rem;
            display: flex;
            flex-direction: column;
            gap: 1rem;
            z-index: 999;
        }

        .floating-btn {
            width: 60px;
            height: 60px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5rem;
            color: var(--white);
            text-decoration: none;
            box-shadow: 0 4px 15px rgba(0,0,0,0.2);
            transition: transform 0.3s;
        }

        .floating-btn:hover {
            transform: scale(1.1);
        }

        .whatsapp-btn {
            background: #25D366;
        }

        .call-btn {
            background: var(--primary-blue);
        }

        /* Footer */
        footer {
            background: var(--dark-grey);
            color: var(--white);
            padding: 3rem 2rem 1rem;
            text-align: center;
        }

        .footer-content {
            max-width: 1200px;
            margin: 0 auto;
        }

        .footer-info {
            margin-bottom: 2rem;
        }

        .footer-info h3 {
            color: var(--primary-blue);
            margin-bottom: 1rem;
        }

        .footer-links {
            margin: 1rem 0;
        }

        .footer-links a {
            color: var(--white);
            text-decoration: none;
            margin: 0 1rem;
            opacity: 0.8;
            transition: opacity 0.3s;
        }

        .footer-links a:hover {
            opacity: 1;
        }

        .copyright {
            border-top: 1px solid rgba(255,255,255,0.1);
            padding-top: 1rem;
            margin-top: 2rem;
            opacity: 0.7;
        }

        /* Success Message */
        .success-message {
            display: none;
            background: var(--success-green);
            color: var(--white);
            padding: 1rem;
            border-radius: 8px;
            margin-bottom: 1rem;
            text-align: center;
        }

        .success-message.show {
            display: block;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
                position: absolute;
                top: 100%;
                left: 0;
                right: 0;
                background: var(--white);
                flex-direction: column;
                padding: 1rem;
                box-shadow: 0 4px 10px rgba(0,0,0,0.1);
            }

            .nav-links.active {
                display: flex;
            }

            .mobile-menu-btn {
                display: block;
            }

            .hero h1 {
                font-size: 2rem;
            }

            .about-content,
            .contact-grid {
                grid-template-columns: 1fr;
            }

            .floating-btns {
                bottom: 1rem;
                right: 1rem;
            }

            .floating-btn {
                width: 50px;
                height: 50px;
                font-size: 1.2rem;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <nav>
            <div class="logo">🚗 Special Driving School</div>
            <button class="mobile-menu-btn" onclick="toggleMenu()">☰</button>
            <ul class="nav-links" id="navLinks">
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#services">Courses</a></li>
                <li><a href="#why-choose">Why Us</a></li>
                <li><a href="#pricing">Pricing</a></li>
                <li><a href="#signup">Enroll Now</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="hero-content">
            <h1>Learn Driving with Confidence in Kolkata</h1>
            <p>Professional driving lessons from experienced instructor Prabhat Ganguli. Safe, affordable, and student-friendly approach to help you master the roads of Kolkata.</p>
            <div class="cta-buttons">
                <a href="#signup" class="btn btn-primary">Enroll Now</a>
                <a href="tel:7003583496" class="btn btn-secondary">📞 Call Now</a>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about">
        <h2 class="section-title">About Special Driving School</h2>
        <div class="about-content">
            <div>
                <p style="margin-bottom: 1rem;">Welcome to Special Driving School, your trusted partner for learning safe and confident driving in Kolkata. We believe that learning to drive should be a pleasant, stress-free experience.</p>
                <p style="margin-bottom: 1rem;">With years of experience teaching students from all backgrounds, we focus on building your confidence behind the wheel while ensuring you understand road safety and traffic rules thoroughly.</p>
                <p>Located in South 24 Parganas, Kolkata, we provide personalized driving lessons tailored to your learning pace and comfort level.</p>
            </div>
            <div class="instructor-card">
                <div style="font-size: 4rem; margin-bottom: 1rem;">👨‍🏫</div>
                <h3>Prabhat Ganguli</h3>
                <p style="font-weight: 600;">Chief Driving Instructor</p>
                <p>Experienced and patient instructor dedicated to making you a safe, confident driver. Specializes in teaching beginners and nervous learners with personalized attention.</p>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" style="background: var(--light-grey);">
        <h2 class="section-title">Our Driving Courses</h2>
        <div class="services-grid">
            <div class="service-card">
                <div class="service-icon">🔰</div>
                <h3>Beginner Driving Course</h3>
                <p>Perfect for first-time learners. Start from basics and build your skills step-by-step with patient guidance.</p>
            </div>
            <div class="service-card">
                <div class="service-icon">🔄</div>
                <h3>Refresher Driving Course</h3>
                <p>Haven't driven in a while? Regain your confidence and update your skills with our refresher program.</p>
            </div>
            <div class="service-card">
                <div class="service-icon">🚙</div>
                <h3>Manual & Automatic Car Training</h3>
                <p>Learn to drive both manual and automatic transmission vehicles based on your preference.</p>
            </div>
            <div class="service-card">
                <div class="service-icon">🛣️</div>
                <h3>Road Safety & Traffic Rules</h3>
                <p>Comprehensive training on Indian traffic rules, road signs, and safe driving practices.</p>
            </div>
        </div>
    </section>

    <!-- Why Choose Us -->
    <section id="why-choose">
        <h2 class="section-title">Why Choose Special Driving School</h2>
        <div class="features-grid">
            <div class="feature-item">
                <div class="feature-icon">⭐</div>
                <h3>Experienced Instructor</h3>
                <p>Learn from Prabhat Ganguli, a skilled instructor with years of teaching experience</p>
            </div>
            <div class="feature-item">
                <div class="feature-icon">🛡️</div>
                <h3>Safe Learning Environment</h3>
                <p>Well-maintained vehicles and emphasis on safety at every step of your learning journey</p>
            </div>
            <div class="feature-item">
                <div class="feature-icon">💰</div>
                <h3>Affordable Pricing</h3>
                <p>Competitive rates with transparent pricing and flexible payment options</p>
            </div>
            <div class="feature-item">
                <div class="feature-icon">📍</div>
                <h3>Local Expertise</h3>
                <p>Deep knowledge of Kolkata roads, traffic patterns, and RTO requirements</p>
            </div>
        </div>
    </section>

    <!-- Pricing Section -->
    <section id="pricing" style="background: var(--light-grey);">
        <h2 class="section-title">Affordable Packages</h2>
        <div class="pricing-grid">
            <div class="pricing-card">
                <h3>Basic Package</h3>
                <div class="price-tag">₹500</div>
                <p style="color: var(--medium-grey); margin-bottom: 1rem;">10 Classes</p>
                <ul class="price-features">
                    <li>10 driving sessions (45 min each)</li>
                    <li>Basic car controls</li>
                    <li>Road safety training</li>
                    <li>Traffic rules guidance</li>
                </ul>
                <a href="#signup" class="btn btn-primary" style="margin-top: 1.5rem; width: 100%;">Select Plan</a>
            </div>
            <div class="pricing-card featured">
                <h3>Standard Package</h3>
                <div class="price-tag">₹6,000</div>
                <p style="color: var(--medium-grey); margin-bottom: 1rem;">20 Classes</p>
                <ul class="price-features">
                    <li>20 driving sessions (45 min each)</li>
                    <li>Complete beginner training</li>
                    <li>Highway driving practice</li>
                    <li>Parking techniques</li>
                    <li>RTO test preparation</li>
                </ul>
                <a href="#signup" class="btn btn-primary" style="margin-top: 1.5rem; width: 100%;">Select Plan</a>
            </div>
            <div class="pricing-card">
                <h3>Advanced Package</h3>
                <div class="price-tag">₹8,500</div>
                <p style="color: var(--medium-grey); margin-bottom: 1rem;">30 Classes</p>
                <ul class="price-features">
                    <li>30 driving sessions (45 min each)</li>
                    <li>Comprehensive training</li>
                    <li>All terrains & conditions</li>
                    <li>Advanced maneuvers</li>
                    <li>Lifetime support</li>
                </ul>
                <a href="#signup" class="btn btn-primary" style="margin-top: 1.5rem; width: 100%;">Select Plan</a>
            </div>
        </div>
        <p style="text-align: center; margin-top: 2rem; color: var(--medium-grey);">
            * Prices are subject to change. Contact us for custom packages.
        </p>
    </section>

    <!-- Testimonials -->
    <section id="testimonials">
        <h2 class="section-title">What Our Students Say</h2>
        <div class="testimonials-grid">
            <div class="testimonial-card">
                <div class="stars">★★★★★</div>
                <p class="testimonial-text">"Prabhat Sir is very patient and explains everything clearly. I was nervous at first but he made me feel comfortable. Now I drive confidently!"</p>
                <p class="testimonial-author">- Ananya S., Kolkata</p>
            </div>
            <div class="testimonial-card">
                <div class="stars">★★★★★</div>
                <p class="testimonial-text">"Best driving school in South 24 Parganas! The instructor is professional and the pricing is very reasonable. Highly recommend!"</p>
                <p class="testimonial-author">- Rajesh M., Salt Lake</p>
            </div>
            <div class="testimonial-card">
                <div class="stars">★★★★★</div>
                <p class="testimonial-text">"I learned driving from zero level. Sir taught me all the basics and helped me pass my driving test on the first attempt. Thank you!"</p>
                <p class="testimonial-author">- Priya D., New Town</p>
            </div>
        </div>
    </section>

    <!-- Signup Section -->
    <section id="signup" style="background: var(--light-grey);">
        <h2 class="section-title">Enroll Now</h2>
        <div class="signup-form">
            <div class="success-message" id="successMessage">
                ✓ Thank you! Your enrollment request has been received. We will contact you shortly to confirm your classes.
            </div>
            <form id="enrollmentForm" onsubmit="handleSubmit(event)">
                <div class="form-group">
                    <label for="name">Full Name *</label>
                    <input type="text" id="name" name="name" required placeholder="Enter your full name">
                </div>
                <div class="form-group">
                    <label for="phone">Phone Number *</label>
                    <input type="tel" id="phone" name="phone" required placeholder="10-digit mobile number" pattern="[0-9]{10}">
                </div>
                <div class="form-group">
                    <label for="email">Email (Optional)</label>
                    <input type="email" id="email" name="email" placeholder="your.email@example.com">
                </div>
                <div class="form-group">
                    <label for="location">Your Location in Kolkata *</label>
                    <input type="text" id="location" name="location" required placeholder="e.g., Salt Lake, New Town, etc.">
                </div>
                <div class="form-group">
                    <label for="course">Select Course *</label>
                    <select id="course" name="course" required>
                        <option value="">Choose a course</option>
                        <option value="basic">Basic Package - 10 Classes (₹500)</option>
                        <option value="standard">Standard Package - 20 Classes (₹6,000)</option>
                        <option value="advanced">Advanced Package - 30 Classes (₹8,500)</option>
                        <option value="custom">Custom Package - Contact for pricing</option>
                    </select>
                </div>
                <div class="form-group">
                    <label for="experience">Previous Driving Experience</label>
                    <select id="experience" name="experience">
                        <option value="none">No experience (Complete beginner)</option>
                        <option value="some">Some experience (Refresher needed)</option>
                        <option value="licensed">Already have license (Practice only)</option>
                    </select>
                </div>
                <div class="form-group">
                    <label for="message">Additional Message (Optional)</label>
                    <textarea id="message" name="message" rows="3" placeholder="Any specific requirements or questions?"></textarea>
                </div>

                <div class="payment-info">
                    <h4>📱 Payment Instructions</h4>
                    <p>After submitting this form, please make the payment via UPI:</p>
                    <div class="upi-id">prabhatganguli196@oksbi</div>
                    <p style="margin-top: 1rem; font-size: 0.9rem;">After payment, we will contact you to schedule your first class.</p>
                </div>

                <button type="submit" class="btn btn-primary" style="width: 100%; padding: 1rem; font-size: 1.1rem;">
                    Submit Enrollment
                </button>
            </form>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact">
        <h2 class="section-title">Contact Us</h2>
        <div class="contact-grid">
            <div>
                <div class="contact-info">
                    <div class="contact-item">
                        <div class="contact-icon">📞</div>
                        <div>
                            <h4>Phone</h4>
                            <a href="tel:7003583496" style="color: var(--primary-blue); text-decoration: none; font-size: 1.2rem;">7003583496</a>
                        </div>
                    </div>
                    <div class="contact-item">
                        <div class="contact-icon">📍</div>
                        <div>
                            <h4>Location</h4>
                            <p>South 24 Parganas<br>Kolkata, West Bengal, India</p>
                        </div>
                    </div>
                    <div class="contact-item">
                        <div class="contact-icon">👨‍🏫</div>
                        <div>
                            <h4>Instructor</h4>
                            <p>Prabhat Ganguli</p>
                        </div>
                    </div>
                </div>
                <div class="map-container">
                    <iframe 
                        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d235850.75765212395!2d88.12665725!3d22.535564600000003!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3a0275ac4337e87b%3A0x17c0530f97e13e9c!2sSouth%2024%20Parganas%2C%20West%20Bengal!5e0!3m2!1sen!2sin!4v1234567890" 
                        width="100%" 
                        height="100%" 
                        style="border:0;" 
                        allowfullscreen="" 
                        loading="lazy">
                    </iframe>
                </div>
            </div>
            <div>
                <form onsubmit="handleContactForm(event)">
                    <div class="form-group">
                        <label for="contact-name">Your Name *</label>
                        <input type="text" id="contact-name" required>
                    </div>
                    <div class="form-group">
                        <label for="contact-phone">Phone Number *</label>
                        <input type="tel" id="contact-phone" required pattern="[0-9]{10}">
                    </div>
                    <div class="form-group">
                        <label for="contact-email">Email</label>
                        <input type="email" id="contact-email">
                    </div>
                    <div class="form-group">
                        <label for="contact-message">Your Message *</label>
                        <textarea id="contact-message" rows="5" required></textarea>
                    </div>
                    <button type="submit" class="btn btn-primary" style="width: 100%;">Send Message</button>
                </form>
            </div>
        </div>
    </section>

    <!-- Floating Action Buttons -->
    <div class="floating-btns">
        <a href="https://wa.me/917003583496?text=Hi,%20I%20want%20to%20learn%20driving" class="floating-btn whatsapp-btn" target="_blank" title="WhatsApp Us">💬</a>
        <a href="tel:7003583496" class="floating-btn call-btn" title="Call Now">📞</a>
    </div>

    <!-- Footer -->
    <footer>
        <div class="footer-content">
            <div class="footer-info">
                <h3>Special Driving School</h3>
                <p>Learn Driving with Confidence</p>
                <p style="margin-top: 1rem;">
                    <strong>Instructor:</strong> Prabhat Ganguli<br>
                    <strong>Phone:</strong> <a href="tel:7003583496" style="color: var(--white);">7003583496</a><br>
                    <strong>Location:</strong> Kolkata, South 24 Parganas, West Bengal
                </p>
            </div>
            <div class="footer-links">
                <a href="#home">Home</a>
                <a href="#about">About</a>
                <a href="#services">Courses</a>
                <a href="#pricing">Pricing</a>
                <a href="#signup">Enroll</a>
                <a href="#contact">Contact</a>
            </div>
            <div class="copyright">
                <p>&copy; 2024 Special Driving School. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <script>
        // Mobile Menu Toggle
        function toggleMenu() {
            const navLinks = document.getElementById('navLinks');
            navLinks.classList.toggle('active');
        }

        // Close menu when clicking a link
        document.querySelectorAll('.nav-links a').forEach(link => {
            link.addEventListener('click', () => {
                document.getElementById('navLinks').classList.remove('active');
            });
        });

        // Enrollment Form Handler
        function handleSubmit(event) {
            event.preventDefault();
            
            // Get form data
            const formData = new FormData(event.target);
            const data = {};
            formData.forEach((value, key) => {
                data[key] = value;
            });

            // Create WhatsApp message with enrollment details
            const message = `🚗 *New Enrollment - Special Driving School*

📝 *Student Details:*
Name: ${data.name}
Phone: ${data.phone}
Email: ${data.email || 'Not provided'}
Location: ${data.location}

📚 *Course Selected:*
${document.querySelector('#course option:checked').text}

🚦 *Experience Level:*
${document.querySelector('#experience option:checked').text}

💬 *Additional Message:*
${data.message || 'None'}

---
Please contact the student to confirm enrollment.`;

            // Send to WhatsApp - opens WhatsApp with pre-filled message
            const whatsappNumber = '917363874647';
            const whatsappURL = `https://wa.me/${whatsappNumber}?text=${encodeURIComponent(message)}`;
            
            // Open WhatsApp in new tab
            window.open(whatsappURL, '_blank');

            // Show success message
            document.getElementById('successMessage').classList.add('show');
            
            // Reset form
            event.target.reset();

            // Scroll to success message
            document.getElementById('successMessage').scrollIntoView({ behavior: 'smooth', block: 'center' });

            // Hide success message after 10 seconds
            setTimeout(() => {
                document.getElementById('successMessage').classList.remove('show');
            }, 10000);
        }

        // Contact Form Handler
        function handleContactForm(event) {
            event.preventDefault();
            alert('Thank you for your message! We will get back to you soon.');
            event.target.reset();
        }

        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });
    </script>
</body>
</html>
