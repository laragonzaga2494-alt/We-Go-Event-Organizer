# We-Go-Event-Organizer
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>

<title>We-Go Event Organizers</title>

<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500;600;700;800&family=Nunito:wght@400;600;700&display=swap" rel="stylesheet">

<style>

:root{
    --green:#1f6b45;
    --lightgreen:#2f8b5c;
    --gold:#d4af37;
    --white:#ffffff;
    --dark:#1b1b1b;
    --gray:#f5f5f5;
}

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

html{
    scroll-behavior:smooth;
}

body{
    font-family:'Nunito', sans-serif;
    background:var(--gray);
    color:#333;
}

/* HEADER */

header{
    position:fixed;
    width:100%;
    top:0;
    left:0;
    z-index:1000;
    padding:18px 8%;
    background:rgba(31,107,69,0.95);
    display:flex;
    justify-content:space-between;
    align-items:center;
    backdrop-filter:blur(10px);
}

.logo{
    font-family:'Montserrat', sans-serif;
    font-size:34px;
    font-weight:800;
    color:var(--gold);
}

.logo span{
    color:var(--white);
}

nav a{
    text-decoration:none;
    color:white;
    margin-left:28px;
    font-size:16px;
    font-weight:700;
    transition:0.3s;
}

nav a:hover{
    color:var(--gold);
}

/* HERO */

.hero{
    min-height:100vh;
    background:
    linear-gradient(rgba(0,0,0,0.55), rgba(0,0,0,0.55)),
    url('https://images.unsplash.com/photo-1519167758481-83f550bb49b3?q=80&w=1800&auto=format&fit=crop');
    background-size:cover;
    background-position:center;
    display:flex;
    justify-content:center;
    align-items:center;
    text-align:center;
    padding:120px 20px;
    color:white;
}

.hero-content{
    max-width:950px;
}

.hero-content h1{
    font-family:'Montserrat', sans-serif;
    font-size:76px;
    line-height:1.1;
    margin-bottom:25px;
}

.hero-content p{
    font-size:22px;
    line-height:1.8;
    margin-bottom:35px;
}

.btn{
    display:inline-block;
    padding:16px 38px;
    border-radius:50px;
    text-decoration:none;
    font-weight:700;
    transition:0.3s;
    font-size:17px;
}

.btn-main{
    background:var(--gold);
    color:var(--dark);
}

.btn-main:hover{
    background:white;
}

/* GENERAL */

section{
    padding:100px 8%;
}

.section-title{
    text-align:center;
    margin-bottom:60px;
}

.section-title h2{
    font-family:'Montserrat', sans-serif;
    font-size:48px;
    color:var(--green);
    margin-bottom:10px;
}

.section-title p{
    font-size:18px;
    color:#666;
}

/* ABOUT */

.about{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:50px;
    align-items:center;
}

.about img{
    width:100%;
    border-radius:25px;
    box-shadow:0 10px 25px rgba(0,0,0,0.15);
}

.about-text h3{
    font-family:'Montserrat', sans-serif;
    font-size:38px;
    color:var(--green);
    margin-bottom:20px;
}

.about-text p{
    line-height:1.9;
    margin-bottom:20px;
    font-size:18px;
}

/* PACKAGES */

.packages{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(300px,1fr));
    gap:30px;
}

.card{
    background:white;
    border-radius:25px;
    overflow:hidden;
    box-shadow:0 8px 20px rgba(0,0,0,0.08);
    transition:0.3s;
}

.card:hover{
    transform:translateY(-10px);
}

.card img{
    width:100%;
    height:240px;
    object-fit:cover;
}

.card-header{
    background:linear-gradient(to right,var(--green),var(--lightgreen));
    padding:30px;
    color:white;
}

.card-header h3{
    font-family:'Montserrat', sans-serif;
    font-size:28px;
}

.card-body{
    padding:30px;
}

.card-body p{
    line-height:1.8;
    margin-bottom:20px;
}

.card-body ul{
    padding-left:20px;
}

.card-body li{
    margin-bottom:12px;
    line-height:1.6;
}

/* BOOKING SECTION */

.booking{
    background:
    linear-gradient(rgba(31,107,69,0.92), rgba(31,107,69,0.92)),
    url('https://images.unsplash.com/photo-1505236858219-8359eb29e329?q=80&w=1600&auto=format&fit=crop');
    background-size:cover;
    background-position:center;
    color:white;
    border-radius:30px;
    padding:70px;
}

.booking h2{
    font-family:'Montserrat', sans-serif;
    text-align:center;
    font-size:50px;
    margin-bottom:15px;
}

.booking p{
    text-align:center;
    margin-bottom:40px;
    font-size:18px;
}

.booking-form{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:25px;
}

.booking-form input,
.booking-form select,
.booking-form textarea{
    width:100%;
    padding:16px;
    border:none;
    border-radius:12px;
    font-size:16px;
    font-family:'Nunito', sans-serif;
}

.booking-form textarea{
    grid-column:1/3;
    resize:none;
    height:140px;
}

.booking-form button{
    grid-column:1/3;
    padding:18px;
    border:none;
    border-radius:50px;
    background:var(--gold);
    color:black;
    font-size:18px;
    font-weight:800;
    cursor:pointer;
    transition:0.3s;
}

.booking-form button:hover{
    background:white;
}

/* CONTACT */

.contact{
    text-align:center;
}

.contact-box{
    background:white;
    border-radius:25px;
    padding:50px;
    max-width:700px;
    margin:auto;
    box-shadow:0 10px 25px rgba(0,0,0,0.08);
}

.contact-box h3{
    font-size:38px;
    color:var(--green);
    margin-bottom:20px;
    font-family:'Montserrat', sans-serif;
}

.contact-box p{
    margin:15px 0;
    font-size:18px;
}

/* FOOTER */

footer{
    background:var(--green);
    color:white;
    text-align:center;
    padding:30px;
    margin-top:50px;
}

/* RESPONSIVE */

@media(max-width:900px){

    nav{
        display:none;
    }

    .hero-content h1{
        font-size:50px;
    }

    .hero-content p{
        font-size:18px;
    }

    .about{
        grid-template-columns:1fr;
    }

    .booking-form{
        grid-template-columns:1fr;
    }

    .booking-form textarea,
    .booking-form button{
        grid-column:1;
    }

    .booking{
        padding:40px 25px;
    }
}

</style>
</head>

<body>

<!-- HEADER -->

<header>

<div class="logo">
WE-GO <span>Events</span>
</div>

<nav>
<a href="#home">Home</a>
<a href="#about">About</a>
<a href="#services">Packages</a>
<a href="#booking">Book Now</a>
<a href="#contact">Contact</a>
</nav>

</header>

<!-- HERO -->

<section class="hero" id="home">

<div class="hero-content">

<h1>Where Elegant Events Come To Life</h1>

<p>
We-Go Event Organizers creates premium, stress-free celebrations with luxury styling,
professional coordination, and unforgettable guest experiences —
all tailored to your vision and budget.
</p>

<a href="#booking" class="btn btn-main">
Book Your Event
</a>

</div>

</section>

<!-- ABOUT -->

<section id="about">

<div class="section-title">
<h2>About We-Go</h2>
<p>Luxury Event Experiences with a Personal Touch</p>
</div>

<div class="about">

<img src="https://images.unsplash.com/photo-1511578314322-379afb476865?q=80&w=1600&auto=format&fit=crop">

<div class="about-text">

<h3>Your Vision, Beautifully Executed</h3>

<p>
At We-Go Event Organizers, we believe every client deserves to enjoy their own celebration without stress.
From intimate gatherings to large-scale luxury events, our team transforms ideas into elegant realities.
</p>

<p>
Our signature approach combines creativity, hospitality, logistics, and premium styling to create seamless events that guests will remember forever.
</p>

<p>
Whether you need day-of coordination or complete full-service management, We-Go is ready to make your event extraordinary.
</p>

</div>

</div>

</section>

<!-- PACKAGES -->

<section id="services">

<div class="section-title">
<h2>Premium Service Packages</h2>
<p>Flexible Event Solutions Designed Around Your Needs</p>
</div>

<div class="packages">

<!-- PACKAGE 1 -->

<div class="card">

<img src="https://images.unsplash.com/photo-1519225421980-715cb0215aed?q=80&w=1200&auto=format&fit=crop"
alt="Essential Coordinator">

<div class="card-header">
<h3>Essential Coordinator</h3>
</div>

<div class="card-body">

<p>
Perfect for prepared planners who need expert day-of execution.
</p>

<ul>
<li>Custom Event Timelines</li>
<li>Vendor Coordination</li>
<li>Setup & Teardown Management</li>
<li>On-Site Event Coordinator</li>
<li>Professional Logistics Handling</li>
</ul>

</div>

</div>

<!-- PACKAGE 2 -->

<div class="card">

<img src="https://images.unsplash.com/photo-1469371670807-013ccf25f16a?q=80&w=1200&auto=format&fit=crop"
alt="Elevated Experience">

<div class="card-header">
<h3>Elevated Experience</h3>
</div>

<div class="card-body">

<p>
Elegant styling combined with smooth operational management.
</p>

<ul>
<li>Planning Assistance</li>
<li>Elegant Event Styling</li>
<li>Decor & Centerpieces</li>
<li>Program Flow Management</li>
<li>Enhanced Guest Experience</li>
</ul>

</div>

</div>

<!-- PACKAGE 3 -->

<div class="card">

<img src="https://images.unsplash.com/photo-1505236858219-8359eb29e329?q=80&w=1200&auto=format&fit=crop"
alt="Grand Celebration">

<div class="card-header">
<h3>Grand Celebration</h3>
</div>

<div class="card-body">

<p>
Luxury full-service event planning for unforgettable celebrations.
</p>

<ul>
<li>A-to-Z Event Planning</li>
<li>Supplier Integration</li>
<li>Premium Styling Concepts</li>
<li>Senior Event Directors</li>
<li>Luxury Guest Experience</li>
</ul>

</div>

</div>

<!-- PACKAGE 4 -->

<div class="card">

<img src="https://images.unsplash.com/photo-1492684223066-81342ee5ff30?q=80&w=1200&auto=format&fit=crop"
alt="Bespoke Collection">

<div class="card-header">
<h3>Bespoke Collection</h3>
</div>

<div class="card-body">

<p>
Fully customized events designed around your imagination.
</p>

<ul>
<li>Custom Culinary Design</li>
<li>Flexible Service Models</li>
<li>Themed Experiences</li>
<li>Adaptive Staffing</li>
<li>Unique Luxury Concepts</li>
</ul>

</div>

</div>

</div>

</section>

<!-- BOOKING -->

<section id="booking">

<div class="booking">

<h2>Book Your Event</h2>

<p>
Tell us about your dream celebration and our team will contact you for a personalized consultation.
</p>

<form class="booking-form"
action="mailto:thomvicente16@gmail.com"
method="POST"
enctype="text/plain">

<input type="text"
name="Full Name"
placeholder="Full Name"
required>

<input type="email"
name="Email Address"
placeholder="Email Address"
required>

<input type="tel"
name="Phone Number"
placeholder="Phone Number"
required>

<select name="Event Type" required>
<option value="">Select Event Type</option>
<option>Wedding</option>
<option>Birthday Celebration</option>
<option>Corporate Event</option>
<option>Anniversary</option>
<option>Private Party</option>
<option>Luxury Gala</option>
<option>Other</option>
</select>

<input type="date"
name="Event Date"
required>

<select name="Preferred Package" required>
<option value="">Preferred Package</option>
<option>Essential Coordinator</option>
<option>Elevated Experience</option>
<option>Grand Celebration</option>
<option>Bespoke Collection</option>
</select>

<textarea
name="Event Details"
placeholder="Tell us about your event vision, guest count, preferred theme, and special requests..."></textarea>

<button type="submit">
Submit Booking Request
</button>

</form>

</div>

</section>

<!-- CONTACT -->

<section id="contact" class="contact">

<div class="section-title">
<h2>Contact Us</h2>
<p>Let's Create Something Extraordinary Together</p>
</div>

<div class="contact-box">

<h3>We-Go Event Organizers</h3>

<p><strong>Email:</strong> thomvicente16@gmail.com</p>

<p><strong>Phone:</strong> +63 907 747 2017</p>

<p><strong>Facebook:</strong> We-Go Event Organizers</p>

<p><strong>Location:</strong> Philippines</p>

</div>

</section>

<!-- FOOTER -->

<footer>

<p>
© 2026 We-Go Event Organizers | Premium Event Management Services
</p>

</footer>

</body>
</html>
