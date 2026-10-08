# Index.html

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>LearnHub - Online Courses</title>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: Arial, sans-serif;
    color: #172033;
    background: #f8faff;
    line-height: 1.6;
}

/* NAVBAR */
header {
    height: 75px;
    padding: 0 8%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    background: white;
    position: sticky;
    top: 0;
    z-index: 100;
    box-shadow: 0 2px 15px rgba(0,0,0,0.05);
}

.logo {
    font-size: 26px;
    font-weight: bold;
    color: #5b5bea;
}

nav {
    display: flex;
    gap: 30px;
}

nav a {
    text-decoration: none;
    color: #172033;
    font-weight: 500;
}

nav a:hover {
    color: #5b5bea;
}

.login-btn {
    border: none;
    padding: 10px 22px;
    border-radius: 8px;
    background: #eeeeff;
    color: #5b5bea;
    font-weight: bold;
    cursor: pointer;
}

/* HERO */
.hero {
    min-height: 600px;
    padding: 80px 8%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 50px;
    background: linear-gradient(135deg, #f5f5ff, #eef7ff);
}

.hero-text {
    max-width: 600px;
}

.tag {
    font-size: 13px;
    font-weight: bold;
    letter-spacing: 2px;
    color: #5b5bea;
}

.hero h1 {
    font-size: 55px;
    line-height: 1.1;
    margin: 18px 0;
}

.hero-text > p:not(.tag) {
    color: #626b7d;
    font-size: 18px;
    margin-bottom: 25px;
}

.primary-btn {
    padding: 14px 28px;
    border: none;
    border-radius: 8px;
    background: #5b5bea;
    color: white;
    font-size: 15px;
    font-weight: bold;
    cursor: pointer;
}

.primary-btn:hover {
    background: #4545c9;
}

/* HERO CARD */
.hero-card {
    width: 350px;
    height: 350px;
    border-radius: 30px;
    padding: 45px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    background: white;
    box-shadow: 0 20px 50px rgba(60,60,120,0.15);
}

.play {
    width: 65px;
    height: 65px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    background: #5b5bea;
    color: white;
    font-size: 25px;
    margin-bottom: 30px;
}

/* COURSES */
.courses {
    padding: 90px 8%;
    background: white;
}

.section-title {
    text-align: center;
    margin-bottom: 45px;
}

.section-title p {
    font-size: 13px;
    font-weight: bold;
    letter-spacing: 2px;
    color: #5b5bea;
}

.section-title h2 {
    font-size: 38px;
    margin-top: 8px;
}

.course-container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 25px;
}

.course-card {
    overflow: hidden;
    border-radius: 15px;
    background: white;
    border: 1px solid #e8eaf0;
    transition: 0.3s;
}

.course-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 15px 35px rgba(0,0,0,0.1);
}

.course-image {
    height: 180px;
    display: flex;
    align-items: center;
    justify-content: center;
    background: #eeeeff;
    color: #5b5bea;
    font-size: 28px;
    font-weight: bold;
}

.course-content {
    padding: 25px;
}

.course-content span {
    font-size: 12px;
    padding: 5px 10px;
    border-radius: 20px;
    background: #eeeeff;
    color: #5b5bea;
}

.course-content h3 {
    margin: 15px 0 8px;
}

.course-content p {
    color: #687083;
}

.course-content button {
    margin-top: 18px;
    padding: 11px 18px;
    border: none;
    border-radius: 7px;
    background: #172033;
    color: white;
    cursor: pointer;
}

.course-content button:hover {
    background: #5b5bea;
}

/* ABOUT */
.about {
    padding: 90px 8%;
    text-align: center;
}

.about h2 {
    font-size: 38px;
}

.about > p {
    max-width: 650px;
    margin: 15px auto 40px;
    color: #687083;
}

.features {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 25px;
}

.features div {
    padding: 30px;
    background: white;
    border-radius: 15px;
    border: 1px solid #e8eaf0;
}

.features h3 {
    margin-bottom: 8px;
}

.features p {
    color: #687083;
}

/* FOOTER */
footer {
    padding: 45px;
    text-align: center;
    background: #172033;
    color: white;
}

footer h3 {
    font-size: 24px;
    margin-bottom: 8px;
}

footer p {
    color: #b9c0ce;
}

/* MOBILE */
@media (max-width: 800px) {

    nav {
        display: none;
    }

    .hero {
        flex-direction: column;
        text-align: center;
        padding: 60px 6%;
    }

    .hero h1 {
        font-size: 40px;
    }

    .hero-card {
        width: 100%;
        max-width: 350px;
    }

    .course-container,
    .features {
        grid-template-columns: 1fr;
    }

    .courses,
    .about {
        padding: 60px 6%;
    }
}
</style>
</head>

<body>

<!-- NAVIGATION -->
<header>

    <div class="logo">LearnHub</div>

    <nav>
        <a href="#home">Home</a>
        <a href="#courses">Courses</a>
        <a href="#about">About</a>
        <a href="#contact">Contact</a>
    </nav>

    <button class="login-btn" onclick="login()">
        Login
    </button>

</header>


<!-- HERO SECTION -->
<section class="hero" id="home">

    <div class="hero-text">

        <p class="tag">LEARN • GROW • SUCCEED</p>

        <h1>
            Upgrade Your Skills With Online Learning
        </h1>

        <p>
            Learn practical skills from beginner to advanced
            level with carefully designed courses.
        </p>

        <button class="primary-btn" onclick="scrollToCourses()">
            Explore Courses
        </button>

    </div>


    <div class="hero-card">

        <div class="play">▶</div>

        <h2>Learn at Your Own Pace</h2>

        <p>
            Flexible learning designed to help you
            achieve your goals.
        </p>

    </div>

</section>


<!-- COURSES -->
<section class="courses" id="courses">

    <div class="section-title">

        <p>OUR COURSES</p>

        <h2>Popular Courses</h2>

    </div>


    <div class="course-container">


        <!-- COURSE 1 -->
        <div class="course-card">

            <div class="course-image">
                HTML & CSS
            </div>

            <div class="course-content">

                <span>Beginner</span>

                <h3>Web Development Basics</h3>

                <p>
                    Build modern and responsive websites
                    using HTML and CSS.
                </p>

                <button onclick="enroll('Web Development Basics')">
                    Enroll Now
                </button>

            </div>

        </div>


        <!-- COURSE 2 -->
        <div class="course-card">

            <div class="course-image">
                JAVA
            </div>

            <div class="course-content">

                <span>Intermediate</span>

                <h3>Java Programming</h3>

                <p>
                    Learn Java fundamentals and
                    object-oriented programming.
                </p>

                <button onclick="enroll('Java Programming')">
                    Enroll Now
                </button>

            </div>

        </div>


        <!-- COURSE 3 -->
        <div class="course-card">

            <div class="course-image">
                SQL
            </div>

            <div class="course-content">

                <span>Beginner</span>

                <h3>SQL & Databases</h3>

                <p>
                    Understand databases and learn
                    to write SQL queries.
                </p>

                <button onclick="enroll('SQL & Databases')">
                    Enroll Now
                </button>

            </div>

        </div>

    </div>

</section>


<!-- ABOUT -->
<section class="about" id="about">

    <h2>Why LearnHub?</h2>

    <p>
        We make learning simple, practical and accessible.
        Learn industry-relevant skills and build your confidence
        through hands-on practice.
    </p>


    <div class="features">

        <div>
            <h3>🎯 Practical Learning</h3>
            <p>
                Learn through real-world examples
                and practical projects.
            </p>
        </div>


        <div>
            <h3>💻 Flexible Access</h3>
            <p>
                Learn anytime and anywhere
                at your own pace.
            </p>
        </div>


        <div>
            <h3>🚀 Career Focused</h3>
            <p>
                Build skills that support
                your career growth.
            </p>
        </div>

    </div>

</section>


<!-- FOOTER -->
<footer id="contact">

    <h3>LearnHub</h3>

    <p>
        Start learning. Start growing.
    </p>

    <p>
        © 2026 LearnHub
    </p>

</footer>


<script>

function scrollToCourses() {

    document.getElementById("courses")
    .scrollIntoView({
        behavior: "smooth"
    });

}


function enroll(course) {

    alert(
        "You selected: " + course +
        "\nThank you for your interest!"
    );

}


function login() {

    alert(
        "Login feature coming soon!"
    );

}

</script>

</body>
</html>
