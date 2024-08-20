Here's how you can style your portfolio using Bootstrap for a responsive design, along with custom CSS for additional visual enhancements. This implementation includes a dark theme, cards for your projects, and a polished layout.

### 1. **HTML Structure**
Ensure that Bootstrap is included in your project, and then integrate the HTML code into your `index.md` or main HTML file.

```html
---
title: "Name"
layout: default
---

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio</title>
    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
    <!-- Font Awesome for icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <!-- Custom CSS -->
    <link rel="stylesheet" href="styles.css">
</head>
<body class="bg-dark text-white">
    <div class="container">
        <header class="text-center my-5">
            <h1 class="display-4">Welcome to My Portfolio</h1>
            <p class="lead">Hello! I'm <strong>Name</strong>, a Computer Science student aspiring to be a Machine Learning Software Engineer. Welcome to my portfolio website, where you can learn more about my projects and skills.</p>
        </header>

        <section class="mb-5">
            <h2 class="h3">About Me</h2>
            <p>My love for technology began in high school, where I studied Computer Science, Mathematics, and Physics at A-level, achieving distinctions. This early passion for tech's potential to solve real-world problems led me to pursue a Bachelor of Science in Computer Science at Africa University, where I’ve maintained a 3.8 GPA. My academic journey has been enriched by deep dives into machine learning, deep learning, and web development.</p>
            <p>Throughout my studies, I’ve worked on various projects that blend theory with practical application. One standout project was a Django event management web app, which enhanced my backend development, machine learning and database management skills. I also completed school and capstone projects like an automatic vehicle recognition system and a course recommender system using Streamlit, showcasing my ability to harness AI and ML to tackle complex challenges.</p>
            <p>My passion extends beyond the classroom. I continuously explore cutting-edge technologies and stay updated on the latest advancements. My interests in AI, ML, Data Science, and Software Engineering are not just academic—they drive my vision of shaping a future where technology enhances human capabilities and improves lives.</p>
        </section>

        <section class="mb-5">
            <h2 class="h3">Education</h2>
            <div class="card bg-secondary mb-3">
                <div class="card-body">
                    <h4 class="card-title">Africa University</h4>
                    <p class="card-text">Computer Science Undergraduate - Expected Graduation Date: June 2026</p>
                    <p class="card-text">GPA: 3.8/4.0</p>
                </div>
            </div>
            <div class="card bg-secondary">
                <div class="card-body">
                    <h4 class="card-title">Thornhill High School (2016 - 2021)</h4>
                    <p class="card-text">Advanced Level (Zimsec) : 2020-2021</p>
                    <p class="card-text">Grades: Pure Mathematics (A), Physics (A), Computer Science (A)</p>
                    <p class="card-text"><strong>Activities:</strong></p>
                    <ul>
                        <li>Midlands Province Chess Team (2016-2017)</li>
                        <li>Interact Club</li>
                        <li>Chess Club (Captain: 2016-2021)</li>
                    </ul>
                </div>
            </div>
        </section>

        <section class="mb-5">
            <h2 class="h3">Certifications</h2>
            <ul class="list-group list-group-flush bg-dark">
                <li class="list-group-item bg-secondary text-white">IBM AI Developer Professional Certificate (Completed: July 29, 2024)</li>
                <li class="list-group-item bg-secondary text-white">Deep Learning Specialization (Completed: July 7, 2024)</li>
                <li class="list-group-item bg-secondary text-white">IBM Machine Learning Professional Certificate (Completed: June 10, 2024)</li>
                <li class="list-group-item bg-secondary text-white">Andrew Ng's Machine Learning Specialization (Completed: May 13, 2024)</li>
                <li class="list-group-item bg-secondary text-white">CS50 Intro to AI (Completed: March 13, 2024)</li>
            </ul>
        </section>

        <section class="mb-5">
            <h2 class="h3">Projects</h2>
            <div class="row">
                <div class="col-md-6 col-lg-4 mb-4">
                    <div class="card bg-secondary text-white">
                        <div class="card-header"><h5>Django Event Management Web App</h5></div>
                        <div class="card-body">
                            <p class="card-text">A comprehensive web application for managing events with features like user registration, email notifications, and sentiment analysis.</p>
                            <a href="#" class="btn btn-primary">View Project</a>
                        </div>
                    </div>
                </div>
                <div class="col-md-6 col-lg-4 mb-4">
                    <div class="card bg-secondary text-white">
                        <div class="card-header"><h5>Automatic Vehicle Recognition System</h5></div>
                        <div class="card-body">
                            <p class="card-text">A Flask-based system integrating OpenCV for real-time vehicle plate detection and recognition.</p>
                            <a href="#" class="btn btn-primary">View Project</a>
                        </div>
                    </div>
                </div>
                <div class="col-md-6 col-lg-4 mb-4">
                    <div class="card bg-secondary text-white">
                        <div class="card-header"><h5>Machine Learning Capstone</h5></div>
                        <div class="card-body">
                            <p class="card-text">A complete Streamlit app developed as part of the IBM Machine Learning Capstone, featuring model training and evaluation.</p>
                            <a href="#" class="btn btn-primary">View Project</a>
                        </div>
                    </div>
                </div>
                <div class="col-md-6 col-lg-4 mb-4">
                    <div class="card bg-secondary text-white">
                        <div class="card-header"><h5>AI Capstone Project with Deep Learning</h5></div>
                        <div class="card-body">
                            <p class="card-text">An AI Capstone Project that involved using pretraining on ResNet and VGG models, achieving high accuracy on the test set.</p>
                            <a href="#" class="btn btn-primary">View Project</a>
                        </div>
                    </div>
                </div>
                <div class="col-md-6 col-lg-4 mb-4">
                    <div class="card bg-secondary text-white">
                        <div class="card-header"><h5>Applied Data Science Capstone</h5></div>
                        <div class="card-body">
                            <p class="card-text">A capstone project involving data collection, analysis, and visualization using SpaceX API and Wikipedia datasets.</p>
                            <a href="#" class="btn btn-primary">View Project</a>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section class="mb-5">
            <h2 class="h3">Skills</h2>
            <ul class="list-unstyled">
                <li><strong>Programming Languages:</strong> Python, JavaScript, C++, SQL</li>
                <li><strong>Frameworks:</strong> Django, Flask, Plotly Dash</li>
                <li><strong>Libraries:</strong> OpenCV, EasyOCR, TensorFlow, Scikit-learn, Pandas, Numpy</li>
                <li><strong>Tools:</strong> Git, Docker, Jupyter Notebook, MySQL</li>
                <li><strong>Other:</strong> Data Science, Machine Learning, Deep Learning, Computer Vision</li>
            </ul>
        </section>

        <section class="mb-5">
            <h2 class="h3">Contact</h2>
            <p>Feel free to reach out to me via <a href="https://www.linkedin.com" class="text-white"><i class="fab fa-linkedin"></i> LinkedIn</a> or email me at <a href="mailto:email@example.com" class="text-white"><i class="fas fa-envelope"></i> email@example.com</a>.</p>
        </section>

        <section>
            <h2 class="h3">Links</h2>
            <ul class="list-unstyled">
                <li><strong>GitHub Repository:</strong> <a href="https://github.com/username" class="text-white">GitHub Profile</a></li>
                <li><strong>Coursera Profile:</strong> <a href="https://www.coursera.org/user"
