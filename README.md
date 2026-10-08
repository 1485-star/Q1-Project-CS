<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>StudyHub - Smart Study Planner</title>

<style>
* {
margin: 0;
padding: 0;
box-sizing: border-box;
scroll-behavior: smooth;
}

body {
font-family: Arial, Helvetica, sans-serif;
background: #f5f5ff;
color: #222;
line-height: 1.6;
}

/* ================= NAVBAR ================= */

nav {
background: white;
padding: 15px 7%;
display: flex;
align-items: center;
justify-content: space-between;
position: sticky;
top: 0;
z-index: 1000;
box-shadow: 0 3px 15px rgba(0,0,0,0.1);
}

.logo {
font-size: 28px;
font-weight: bold;
color: #6c20d9;
}

.logo span {
color: #222;
}

nav ul {
list-style: none;
display: flex;
gap: 30px;
}

nav ul li a {
text-decoration: none;
color: #222;
font-weight: bold;
transition: 0.3s;
}

nav ul li a:hover {
color: #6c20d9;
}

/* ================= HERO ================= */

.hero {
min-height: 650px;
padding: 70px 8%;
display: flex;
align-items: center;
justify-content: space-between;
gap: 50px;
background: linear-gradient(135deg, #ffffff, #eee7ff);
}

.hero-text {
flex: 1;
}

.hero-text h1 {
font-size: 65px;
color: #37138f;
margin-bottom: 10px;
}

.hero-text h1 span {
color: #8b22ed;
}

.hero-text h2 {
font-size: 28px;
color: #333;
margin-bottom: 20px;
}

.hero-text p {
font-size: 19px;
max-width: 600px;
margin-bottom: 30px;
color: #444;
}

.download-btn {
display: inline-block;
text-decoration: none;
background: linear-gradient(135deg, #7415ed, #a52bff);
color: white;
padding: 15px 35px;
border-radius: 35px;
font-size: 20px;
font-weight: bold;
box-shadow: 0 8px 20px rgba(117, 24, 230, 0.3);
transition: 0.3s;
}

.download-btn:hover {
transform: translateY(-4px);
}

.phone-container {
flex: 1;
display: flex;
justify-content: center;
}

.phone {
width: 280px;
height: 560px;
background: #111;
border: 10px solid #111;
border-radius: 45px;
box-shadow: 0 20px 40px rgba(0,0,0,0.3);
overflow: hidden;
transform: rotate(3deg);
}

.phone-screen {
height: 100%;
background: linear-gradient(180deg, #f4eaff, #ffffff);
padding: 30px 15px;
}

.phone-screen h3 {
color: #6017cf;
text-align: center;
font-size: 25px;
margin-bottom: 25px;
}

.task {
background: white;
padding: 15px;
border-radius: 15px;
margin: 12px 0;
box-shadow: 0 4px 12px rgba(0,0,0,0.1);
}

.task strong {
color: #42129d;
}

/* ================= FEATURES BAR ================= */

.features-bar {
background: white;
padding: 30px 8%;
display: grid;
grid-template-columns: repeat(5, 1fr);
gap: 20px;
text-align: center;
box-shadow: 0 3px 15px rgba(0,0,0,0.08);
}

.feature-icon {
font-size: 40px;
margin-bottom: 8px;
}

.features-bar h3 {
color: #333;
font-size: 17px;
}

/* ================= GENERAL SECTION ================= */

section {
padding: 70px 8%;
}

.section-title {
text-align: center;
color: #4814a8;
font-size: 40px;
margin-bottom: 45px;
}

/* ================= ABOUT ================= */

.about {
display: flex;
align-items: center;
gap: 50px;
}

.about-text {
flex: 1;
}

.about-text h2 {
color: #40129b;
font-size: 35px;
margin-bottom: 20px;
}

.about-text p {
font-size: 18px;
color: #444;
}

.students-image {
flex: 1;
min-height: 300px;
border-radius: 25px;
background: linear-gradient(135deg, #d9c5ff, #f7f2ff);
display: flex;
align-items: center;
justify-content: center;
font-size: 90px;
box-shadow: 0 10px 30px rgba(0,0,0,0.1);
}

/* ================= KEY FEATURES ================= */

.feature-section {
background: white;
}

.feature-grid {
display: grid;
grid-template-columns: repeat(3, 1fr);
gap: 25px;
}

.feature-card {
background: #f7f2ff;
padding: 30px;
border-radius: 20px;
transition: 0.3s;
border-left: 6px solid #751ee5;
}

.feature-card:hover {
transform: translateY(-7px);
box-shadow: 0 10px 25px rgba(0,0,0,0.1);
}

.feature-card h3 {
color: #5312b8;
font-size: 22px;
margin-bottom: 10px;
}

.feature-card p {
color: #444;
}

/* ================= LISTS ================= */

.lists-container {
display: grid;
grid-template-columns: 1fr 1fr;
gap: 40px;
}

.list-box {
background: white;
padding: 35px;
border-radius: 20px;
box-shadow: 0 5px 20px rgba(0,0,0,0.08);
}

.list-box h2 {
color: #5312b8;
margin-bottom: 20px;
}

.list-box ul,
.list-box ol {
padding-left: 25px;
}

.list-box li {
margin: 12px 0;
font-size: 17px;
}

/* ================= WHO IS IT FOR ================= */

.target {
background: linear-gradient(135deg, #eee5ff, #ffffff);
text-align: center;
}

.target p {
max-width: 800px;
margin: auto;
font-size: 20px;
}

.target-users {
display: flex;
justify-content: center;
gap: 30px;
margin-top: 35px;
flex-wrap: wrap;
}

.user {
background: white;
padding: 25px 35px;
border-radius: 20px;
box-shadow: 0 5px 15px rgba(0,0,0,0.1);
font-size: 18px;
font-weight: bold;
}

/* ================= CTA ================= */

.cta {
text-align: center;
background: linear-gradient(135deg, #45109e, #8d20e8);
color: white;
}

.cta h2 {
font-size: 45px;
margin-bottom: 15px;
}

.cta p {
font-size: 20px;
margin-bottom: 30px;
}

.cta .download-btn {
background: white;
color: #6115c8;
}

/* ================= CONTACT ================= */

.contact {
text-align: center;
background: white;
}

.contact p {
font-size: 18px;
margin: 10px 0;
}

/* ================= FOOTER ================= */

footer {
background: #17101f;
color: white;
text-align: center;
padding: 25px;
}

footer strong {
color: #a335ff;
}

/* ================= RESPONSIVE ================= */

@media (max-width: 900px) {

nav ul {
gap: 12px;
}

.hero {
flex-direction: column;
text-align: center;
}

.hero-text h1 {
font-size: 50px;
}

.features-bar {
grid-template-columns: repeat(2, 1fr);
}

.about {
flex-direction: column;
}

.feature-grid {
grid-template-columns: 1fr 1fr;
}
}

@media (max-width: 600px) {

nav {
flex-direction: column;
gap: 15px;
}

nav ul {
flex-wrap: wrap;
justify-content: center;
}

.hero-text h1 {
font-size: 42px;
}

.hero-text h2 {
font-size: 23px;
}

.features-bar {
grid-template-columns: 1fr 1fr;
}

.feature-grid {
grid-template-columns: 1fr;
}

.lists-container {
grid-template-columns: 1fr;
}

.phone {
width: 230px;
height: 460px;
}

.section-title {
font-size: 32px;
}
}
</style>
</head>

<body>

<!-- ================= NAVIGATION ================= -->

<nav>
<div class="logo">
Study<span>Hub</span>
</div>

<ul>
<li><a href="#home">Home</a></li>
<li><a href="#features">Features</a></li>
<li><a href="#how">How It Works</a></li>
<li><a href="#download">Download</a></li>
<li><a href="#contact">Contact</a></li>
</ul>
</nav>


<!-- ================= HERO / INTRODUCTION ================= -->

<section class="hero" id="home">

<div class="hero-text">

<h1>Study<span>Hub</span></h1>

<h2>Plan • Organize • Achieve</h2>

<p>
StudyHub is a smart study planner app that helps
students organize their time, stay focused, and
achieve their academic goals easily.
</p>

<a href="#download" class="download-btn">
Download Now
</a>

</div>


<!-- App Screen -->

<div class="phone-container">

<div class="phone">

<div class="phone-screen">

<h3>StudyHub</h3>

<div class="task">
<strong>Math Homework</strong>
<br>
Today
</div>

<div class="task">
<strong>Science Project</strong>
<br>
Tomorrow
</div>

<div class="task">
<strong>Read Book</strong>
<br>
Friday
</div>

<div class="task">
<strong>Study Session</strong>
<br>
5:00 PM
</div>

</div>

</div>

</div>

</section>


<!-- ================= FEATURES BAR ================= -->

<div class="features-bar">

<div>
<div class="feature-icon">📅</div>
<h3>Smart Planner</h3>
</div>

<div>
<div class="feature-icon">🔔</div>
<h3>Task Reminders</h3>
</div>

<div>
<div class="feature-icon">📊</div>
<h3>Progress Tracker</h3>
</div>

<div>
<div class="feature-icon">📖</div>
<h3>Study Resources</h3>
</div>

<div>
<div class="feature-icon">🎯</div>
<h3>Personalized Goals</h3>
</div>

</div>


<!-- ================= TARGET USERS ================= -->

<section class="target" id="users">

<h2 class="section-title">
Who is it for?
</h2>

<p>
StudyHub is designed for students, teachers,
and anyone who wants to become more organized,
focused, and productive.
</p>

<div class="target-users">

<div class="user">
🎓 Students
</div>

<div class="user">
👨‍🏫 Teachers
</div>

<div class="user">
📚 Study Groups
</div>

<div class="user">
🎯 Goal-Oriented People
</div>

</div>

</section>


<!-- ================= KEY FEATURES ================= -->

<section class="feature-section" id="features">

<h2 class="section-title">
Key Features
</h2>

<div class="feature-grid">

<div class="feature-card">
<h3>📅 Smart Study Planner</h3>
<p>
Create a study schedule and organize
your subjects and assignments easily.
</p>
</div>

<div class="feature-card">
<h3>🔔 Task Reminders</h3>
<p>
Get reminders and notifications so
you never forget an important task.
</p>
</div>

<div class="feature-card">
<h3>📊 Progress Tracker</h3>
<p>
Track your study progress and see
how much you have achieved.
</p>
</div>

<div class="feature-card">
<h3>🎯 Personalized Goals</h3>
<p>
Set academic goals and work toward
them step by step.
</p>
</div>

<div class="feature-card">
<h3>📚 Study Resources</h3>
<p>
Keep useful study materials and
resources organized in one place.
</p>
</div>

<div class="feature-card">
<h3>✨ Easy Design</h3>
<p>
A clean and simple interface makes
StudyHub easy for everyone to use.
</p>
</div>

</div>

</section>


<!-- ================= HOW TO USE ================= -->

<section id="how">

<h2 class="section-title">
How to Use StudyHub
</h2>

<div class="lists-container">

<!-- Unordered List -->

<div class="list-box">

<h2>Key Features</h2>

<ul>
<li>Smart study planner</li>
<li>Task reminders and notifications</li>
<li>Progress tracker</li>
<li>Personalized goals</li>
<li>Access to study resources</li>
<li>Clean and easy-to-use design</li>
</ul>

</div>


<!-- Ordered List -->

<div class="list-box">

<h2>How to Use</h2>

<ol>
<li>Download the app from the App Store or Google Play.</li>
<li>Create an account.</li>
<li>Set your study goals.</li>
<li>Add your tasks and reminders.</li>
<li>Start planning and achieve your goals.</li>
</ol>

</div>

</div>

</section>


<!-- ================= EXTRA INFORMATION ================= -->

<section class="target">

<h2 class="section-title">
Why Choose StudyHub?
</h2>

<p>
Studying can become difficult when you have many
assignments, exams, and projects. StudyHub puts
everything you need in one simple place. With
planning tools, reminders, progress tracking,
and personalized goals, students can spend less
time worrying about organization and more time
focusing on learning.
</p>

</section>


<!-- ================= DOWNLOAD ================= -->

<section class="cta" id="download">

<h2>
Plan Today for a Brighter Tomorrow!
</h2>

<p>
Build better study habits and achieve your
academic goals with StudyHub.
</p>

<a href="#" class="download-btn">
Download StudyHub
</a>

</section>


<!-- ================= CONTACT ================= -->

<section class="contact" id="contact">

<h2 class="section-title">
Contact Us
</h2>

<p>
Have a question or suggestion?
</p>

<p>
Email: studyhub@example.com
</p>

<p>
Phone: +20 100 000 0000
</p>

</section>


<!-- ================= FOOTER ================= -->

<footer>

<p>
© 2026 <strong>StudyHub</strong>.
All Rights Reserved.
</p>

<p>
Plan Today • Study Better • Achieve More
</p>

</footer>

</body>
</html>
