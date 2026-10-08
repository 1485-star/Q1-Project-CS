<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>StudyHub - Smart Study Planner</title>

    <style>
        body {
            background-color: #f5f9ff;
            color: #333333;
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }

        header {
            background-color: #4b19a8;
            color: white;
            text-align: center;
            padding: 30px;
        }

        header h1 {
            font-size: 48px;
            margin: 10px;
        }

        header p {
            font-size: 20px;
        }

        nav {
            background-color: #24104f;
            text-align: center;
            padding: 15px;
        }

        nav a {
            color: white;
            text-decoration: none;
            margin: 0 20px;
            font-weight: bold;
        }

        nav a:hover {
            color: #d9b8ff;
        }

        .container {
            width: 85%;
            margin: auto;
        }

        section {
            background-color: white;
            margin: 25px 0;
            padding: 25px;
            border-radius: 15px;
            box-shadow: 0 3px 10px #cccccc;
        }

        h2 {
            color: #4b19a8;
            font-size: 30px;
        }

        p {
            font-size: 18px;
            line-height: 1.7;
        }

        .app-image {
            display: block;
            width: 400px;
            max-width: 90%;
            margin: 20px auto;
            border-radius: 20px;
            box-shadow: 0 5px 15px #aaaaaa;
        }

        ul, ol {
            font-size: 18px;
            line-height: 2;
        }

        li::marker {
            color: #4b19a8;
            font-weight: bold;
        }

        .features {
            display: flex;
            justify-content: space-around;
            gap: 20px;
            flex-wrap: wrap;
        }

        .feature-box {
            background-color: #f0e7ff;
            padding: 20px;
            border-radius: 15px;
            width: 250px;
            text-align: center;
        }

        .feature-box h3 {
            color: #4b19a8;
        }

        .download {
            background-color: #4b19a8;
            color: white;
            text-align: center;
        }

        .download h2 {
            color: white;
        }

        .button {
            display: inline-block;
            background-color: white;
            color: #4b19a8;
            padding: 15px 30px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: bold;
            font-size: 18px;
        }

        .button:hover {
            background-color: #e5d4ff;
        }

        footer {
            background-color: #24104f;
            color: white;
            text-align: center;
            padding: 25px;
            margin-top: 30px;
        }
    </style>
</head>

<body>

    <!-- Page Title -->
    <header>
        <h1>StudyHub</h1>
        <p>Plan • Organize • Achieve</p>
    </header>

    <!-- Navigation -->
    <nav>
        <a href="#home">Home</a>
        <a href="#features">Features</a>
        <a href="#how">How It Works</a>
        <a href="#download">Download</a>
        <a href="#contact">Contact</a>
    </nav>

    <div class="container">

        <!-- Introduction Section -->
        <section id="home">
            <h2>Welcome to StudyHub</h2>

            <p>
                StudyHub is a smart study planner app that helps students
                organize their time, stay focused, and achieve their academic
                goals easily. It brings study planning, reminders, progress
                tracking, and study resources together in one simple app.
            </p>

            <p>
                With StudyHub, students can create personalized study goals,
                manage their homework, receive reminders, and keep track of
                their progress. The app is designed to make studying easier,
                more organized, and more productive.
            </p>

            <!-- App Image -->
            <img
                src="https://images.unsplash.com/photo-1516321318423-f06f85e504b3?auto=format&fit=crop&w=800&q=80"
                alt="Student using technology"
                class="app-image"
                width="400"
            >
        </section>


        <!-- Main Features -->
        <section id="features">

            <h2>Key Features</h2>

            <ul>
                <li>Smart study planner</li>
                <li>Task reminders and notifications</li>
                <li>Progress tracker</li>
                <li>Personalized study goals</li>
                <li>Access to study resources</li>
                <li>Clean and easy-to-use design</li>
            </ul>

            <div class="features">

                <div class="feature-box">
                    <h3>Smart Planner</h3>
                    <p>
                        Organize your study schedule and manage your time
                        effectively.
                    </p>
                </div>

                <div class="feature-box">
                    <h3>Task Reminders</h3>
                    <p>
                        Get reminders about homework, exams, and important
                        assignments.
                    </p>
                </div>

                <div class="feature-box">
                    <h3>Progress Tracker</h3>
                    <p>
                        Track your progress and see how much you have achieved.
                    </p>
                </div>

                <div class="feature-box">
                    <h3>Personalized Goals</h3>
                    <p>
                        Create study goals that match your personal academic
                        needs.
                    </p>
                </div>

            </div>

        </section>


        <!-- How To Use - Ordered List -->
        <section id="how">

            <h2>How to Use StudyHub</h2>

            <ol>
                <li>Download the app from the App Store or Google Play.</li>
                <li>Create an account.</li>
                <li>Set your study goals.</li>
                <li>Add your tasks and reminders.</li>
                <li>Start planning and achieve your goals.</li>
            </ol>

        </section>


        <!-- Target Users -->
        <section>

            <h2>Who Is It For?</h2>

            <p>
                StudyHub is designed for students, teachers, and anyone who
                wants to become more organized and productive. It can help
                students manage homework, prepare for exams, organize their
                schedules, and reach their academic goals.
            </p>

            <!-- Extra Image -->
            <img
                src="https://images.unsplash.com/photo-1523240795612-9a054b0db644?auto=format&fit=crop&w=800&q=80"
                alt="Students studying together"
                class="app-image"
                width="400"
            >

        </section>


        <!-- Why StudyHub -->
        <section>

            <h2>Why Choose StudyHub?</h2>

            <p>
                Studying can sometimes become difficult when students have
                many assignments, exams, and activities to manage. StudyHub
                makes organization easier by keeping everything in one place.
            </p>

            <p>
                Instead of forgetting important tasks, students can use
                StudyHub to plan their day, receive reminders, monitor their
                progress, and stay motivated.
            </p>

        </section>


        <!-- Download Section -->
        <section id="download" class="download">

            <h2>Download StudyHub Today!</h2>

            <p>
                Start planning today for a brighter tomorrow.
            </p>

            <a href="#" class="button">Download Now</a>

        </section>


        <!-- Contact -->
        <section id="contact">

            <h2>Contact Us</h2>

            <p>
                Have questions or suggestions? Contact the StudyHub team and
                let us know how we can make studying easier for you.
            </p>

            <p>
                Email: studyhub@example.com
            </p>

        </section>

    </div>


    <!-- Closing Section -->
    <footer>

        <h2>Plan Today for a Brighter Tomorrow!</h2>

        <p>
            Study smart. Stay organized. Achieve your goals.
        </p>

        <p>
            © 2026 StudyHub
        </p>

    </footer>

</body>
</html>
