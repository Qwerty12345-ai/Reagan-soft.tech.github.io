# Reagan-soft.tech.github.io
#html file
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>EduAI - AI in Schools</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css"/>
  <link rel="stylesheet" href="style.css"/>
</head>
<body>
  <!-- Header Section -->
  <header>
    <nav class="navbar">
      <div class="logo">
        <h1>EduAI</h1>
      </div>
      <ul class="nav-links">
        <li><a href="index.html" class="active">Home</a></li>
        <li><a href="about.html">About</a></li>
        <li><a href="contact.html">Contact</a></li>
      </ul>
      <div class="burger">
        <div class="line"></div>
        <div class="line"></div>
        <div class="line"></div>
      </div>
    </nav>
  </header>

  <!-- Main Content -->
  <main>
    <!-- Hero Section with Slider -->
    <section class="hero">
      <div class="slider-container">
        <div class="slide active">
          <img src="images/ai-classroom.jpg" alt="AI Classroom"/>
          <div class="slide-content">
            <h2>Transforming Education with AI</h2>
            <p>Personalized learning experiences for every student.</p>
          </div>
        </div>
        <div class="slide">
          <img src="images/robot-teacher.jpg" alt="Robot Teacher"/>
          <div class="slide-content">
            <h2>Smart Tutoring Systems</h2>
            <p>24/7 learning assistance powered by artificial intelligence.</p>
          </div>
        </div>
        <!-- Add more slides here if needed -->
        <button class="prev">❮</button>
        <button class="next">❯</button>
      </div>
    </section>

    <!-- Features Section -->
    <section class="features">
      <h2>AI Education Benefits</h2>
      <div class="grid-container">
        <div class="feature-card">
          <i class="fas fa-brain"></i>
          <h3>Adaptive Learning</h3>
          <p>AI systems adjust to each student's unique learning pace.</p>
        </div>
        <div class="feature-card">
          <i class="fas fa-robot"></i>
          <h3>Virtual Assistants</h3>
          <p>Instant homework help anytime, anywhere.</p>
        </div>
        <div class="feature-card">
          <i class="fas fa-chart-line"></i>
          <h3>Progress Tracking</h3>
          <p>Real-time performance insights for students and teachers.</p>
        </div>
      </div>
    </section>
  </main>

  <!-- Footer -->
  <footer>
    <div class="footer-content">
      <div class="social-links">
        <a href="https://github.com/Qwerty12345-ai" target="_blank"><i class="fab fa-github"></i></a>
      </div>
      <p>&copy; 2025 EduAI. All rights reserved.</p>
    </div>
  </footer>
  <section class="contact-section">
  <div class="contact-info">
    <h2>Contact Us</h2>
    <div class="contact-details">
      <p><i class="fas fa-phone"></i> <strong>Phone:</strong> <a href="tel:0711607906">0711 607 906</a></p>
      <p><i class="fas fa-envelope"></i> <strong>Email:</strong> <a href="mailto:reagangrandville6@gmail.com">reagangrandville6@gmail.com</a></p>
      <p><i class="fab fa-github"></i> <strong>GitHub:</strong> <a href="https://github.com/Qwerty12345-ai" target="_blank">Reagan Soft.Tech</a></p>
    </div>
  </div>

  <form class="contact-form" id="contactForm" action="#" method="POST">
    <h2>Send Us a Message</h2>

    <div class="form-group">
      <label for="name">Your Name</label>
      <input type="text" id="name" name="name" placeholder="John Doe" required>
    </div>

    <div class="form-group">
      <label for="email">Your Email</label>
      <input type="email" id="email" name="email" placeholder="example@email.com" required>
    </div>

    <div class="form-group">
      <label for="message">Your Message</label>
      <textarea id="message" name="message" rows="5" placeholder="Write your message here..." required></textarea>
    </div>

    <button type="submit">Send Message</button>
  </form>
</section>


  <!-- JavaScript -->
  <script src="script.js"></script>
</body>
</html>
#css file
/* Base Reset and Font */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Segoe UI', sans-serif;
}

body {
  background-color: #f5f7fb;
  color: #333;
  line-height: 1.6;
}

/* Navbar */
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1.5rem 5%;
  background: linear-gradient(135deg, #2c3e50, #3498db);
  color: white;
  position: relative;
  z-index: 10;
}

.logo h1 {
  font-size: 2rem;
  color: #fff;
}

.nav-links {
  display: flex;
  gap: 2rem;
  list-style: none;
}

.nav-links a {
  color: white;
  text-decoration: none;
  font-weight: 500;
  transition: color 0.3s ease;
}

.nav-links a:hover,
.nav-links a.active {
  color: #ecf0f1;
}

/* Burger menu (hidden by default) */
.burger {
  display: none;
  flex-direction: column;
  gap: 5px;
  cursor: pointer;
}

.burger .line {
  width: 25px;
  height: 3px;
  background-color: white;
  border-radius: 3px;
}

/* Hero Section */
.hero {
  position: relative;
  height: 70vh;
}

.slider-container {
  position: relative;
  height: 100%;
  overflow: hidden;
}

.slide {
  position: absolute;
  width: 100%;
  height: 100%;
  opacity: 0;
  transition: opacity 0.7s ease-in-out;
}

.slide.active {
  opacity: 1;
}

.slide img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  filter: brightness(0.7);
}

.slide-content {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
  color: white;
}

.slide-content h2 {
  font-size: 2.5rem;
  margin-bottom: 1rem;
}

.slide-content p {
  font-size: 1.2rem;
}

/* Slider buttons */
.prev,
.next {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  background: rgba(0, 0, 0, 0.5);
  color: white;
  border: none;
  font-size: 2rem;
  padding: 0.5rem 1rem;
  cursor: pointer;
  z-index: 5;
  border-radius: 50%;
}

.prev {
  left: 20px;
}

.next {
  right: 20px;
}

/* Features Section */
.features {
  padding: 4rem 5%;
  text-align: center;
}

.features h2 {
  font-size: 2rem;
  margin-bottom: 2rem;
}

.grid-container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 2rem;
}

.feature-card {
  background: white;
  padding: 2rem;
  border-radius: 12px;
  text-align: center;
  box-shadow: 0 6px 12px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s, box-shadow 0.3s;
}

.feature-card:hover {
  transform: translateY(-8px);
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.15);
}

.feature-card i {
  font-size: 2.5rem;
  color: #3498db;
  margin-bottom: 1rem;
}

.feature-card h3 {
  margin-bottom: 0.5rem;
  color: #2c3e50;
}

/* Contact Page Styles */
.contact-section {
  padding: 4rem 5%;
  display: flex;
  flex-wrap: wrap;
  gap: 3rem;
}

.contact-info,
.contact-form {
  flex: 1;
  min-width: 300px;
}

.form-group {
  margin-bottom: 1.5rem;
}

input,
textarea {
  width: 100%;
  padding: 0.8rem;
  border: 1px solid #ccc;
  border-radius: 5px;
  font-size: 1rem;
  resize: vertical;
}

button {
  background: #3498db;
  color: white;
  padding: 1rem 2rem;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  transition: background 0.3s;
}

button:hover {
  background: #2980b9;
}

/* Footer */
footer {
  background-color: #2c3e50;
  color: white;
  padding: 2rem 5%;
  text-align: center;
}

.footer-content {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.footer-content .social-links {
  margin-bottom: 1rem;
}

.footer-content a {
  color: white;
  font-size: 1.5rem;
  margin: 0 0.5rem;
  transition: color 0.3s;
}

.footer-content a:hover {
  color: #3498db;
}

/* Responsive */
@media (max-width: 768px) {
  .nav-links {
    display: none;
    position: absolute;
    top: 70px;
    left: 0;
    width: 100%;
    flex-direction: column;
    align-items: center;
    background: #2c3e50;
    padding: 2rem 0;
  }

  .nav-links.active {
    display: flex;
  }

  .burger {
    display: flex;
  }

  .hero {
    height: 50vh;
  }

  .slide-content h2 {
    font-size: 1.8rem;
  }

  .slide-content p {
    font-size: 1rem;
  }
}

 # jss file
 // =======================
// Navigation Toggle (Burger Menu)
// =======================
document.addEventListener('DOMContentLoaded', () => {
  const burger = document.querySelector('.burger');
  const navLinks = document.querySelector('.nav-links');

  burger.addEventListener('click', () => {
    navLinks.classList.toggle('active');
    burger.classList.toggle('toggle');
  });
});

// =======================
// Image Slider Functionality
// =======================
let currentSlide = 0;
const slides = document.querySelectorAll('.slide');
const prevBtn = document.querySelector('.prev');
const nextBtn = document.querySelector('.next');

function showSlide(index) {
  slides.forEach((slide, i) => {
    slide.classList.remove('active');
    if (i === index) {
      slide.classList.add('active');
    }
  });
}

function nextSlide() {
  currentSlide = (currentSlide + 1) % slides.length;
  showSlide(currentSlide);
}

function prevSlide() {
  currentSlide = (currentSlide - 1 + slides.length) % slides.length;
  showSlide(currentSlide);
}

// Auto-slide every 5 seconds
let autoSlideInterval = setInterval(nextSlide, 500

# Documentation
AI for schools Curriculumn

#Languages
#HTML
#CSS
#JSS

# purpose for AI in schools and learning
Artificial intelligence (AI) offers a multitude of benefits for schools, transforming the educational landscape for students, teachers, and administrators alike. These advantages range from highly personalized learning experiences to increased efficiency in school operations.

For Students:

Personalized Learning: AI can tailor educational content to meet the unique needs and learning styles of each student. By analyzing individual strengths, weaknesses, and pace, AI-driven platforms can provide customized lesson plans, resources, and feedback. This allows students to learn at their own speed, fostering better engagement and understanding.
Enhanced Engagement and Motivation: AI can make learning more interactive and enjoyable through tools like educational games, virtual reality (VR), augmented reality (AR), and intelligent tutoring systems. These technologies can create immersive learning experiences, making complex concepts more understandable and boosting student motivation.
Immediate Feedback and Support: AI systems can provide students with instantaneous and detailed feedback on their work, helping them identify areas for improvement and reinforcing learning. AI-powered tutors and chatbots can also offer 24/7 assistance, answering questions and providing guidance when teachers are unavailable.
Improved Learning Outcomes: By identifying learning gaps and providing targeted interventions, AI can help students achieve better academic results. Continuous evaluation and data analytics enable AI to adapt teaching strategies and resources to optimize learning.
Accessibility for All Learners: AI offers powerful tools to support students with special needs and diverse learning requirements. Features like text-to-speech, speech recognition, and translation services can make educational materials more accessible, promoting inclusivity in the classroom.
Preparation for the Future: Exposure to AI-powered tools and technologies in the classroom can help prepare students for the future workforce, where AI is increasingly prevalent.
For Teachers:

Reduced Administrative Workload: AI can automate time-consuming administrative tasks such as grading, scheduling, managing student records, and tracking attendance. This frees up teachers to focus more on instruction, student interaction, and professional development.
Support in Lesson Planning and Content Creation: AI tools can assist teachers in developing lesson plans, creating engaging activities and assessments, and finding relevant educational resources. This can save teachers significant time and effort.
Data-Driven Insights: AI can analyze student performance data to provide teachers with valuable insights into learning patterns, identify students who may be struggling, and understand areas where teaching strategies may need adjustment.
Differentiated Instruction: AI can help teachers differentiate instruction by providing resources and tools to tailor lessons to the varying abilities and learning styles within a classroom.
Enhanced Creativity and Collaboration: By automating routine tasks, AI can give teachers more time to focus on creative teaching methods and collaborate with colleagues to share best practices.
For School Administration:

Increased Efficiency: AI can streamline various administrative processes, including admissions and enrollment, resource allocation (classrooms, equipment, staff), financial management, and communication with parents.
Improved Decision-Making: AI can analyze large datasets to provide administrators with actionable insights for strategic planning, policy-making, and improving overall school performance.
Efficient Resource Management: AI tools can help optimize the use of school resources, potentially reducing operational costs.
Enhanced Communication: AI-powered chatbots and virtual assistants can handle routine inquiries from students, parents, and staff, providing quick and accurate responses.
Improved Campus Security: AI can enhance campus safety through advanced surveillance systems and threat detection algorithms.
 
