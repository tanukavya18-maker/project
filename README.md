# Project Responsive Web Design using Bootstrap
# Date:24-12-2025
# AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.

# DESIGN STEPS:
## Step 1:
Clone the repository from GitHub.

## Step 2:
Create Django Admin project.

## Step 3:
Create a New App under the Django Admin project.

## Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

## Step 5:
Create a HTML file and include the needed Bootstrap components.

## Step 6:
Publish the website in the LocalHost.

# PROGRAM :
```
<html>
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Nammatech Solutions</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet"/>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons/font/bootstrap-icons.css">
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
    }
    .hero {
      background: url('https://images.unsplash.com/photo-1504384308090-c894fdcc538d') center center/cover no-repeat;
      color: white;
      text-align: center;
      padding: 150px 0;
      position: relative;
    }
    .hero::after {
      content: "";
      position: absolute;
      top: 0; left: 0; right: 0; bottom: 0;
      background-color: rgba(0, 0, 0, 0.5);
    }
    .hero-content {
      position: relative;
      z-index: 1;
    }
    .service-card:hover {
      transform: translateY(-8px);
      transition: 0.3s;
    }
    .testimonial img {
      width: 60px;
      border-radius: 50%;
    }
    .gallery-img {
      width: 100%;
      height: 200px;
      object-fit: cover;
    }
  </style>
</head>
<body>

<!-- Navbar -->
<nav class="navbar navbar-expand-lg navbar-dark bg-dark sticky-top">
  <div class="container">
    <a class="navbar-brand fw-bold" href="#">
    </a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
      data-bs-target="#navbarNav">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
      <ul class="navbar-nav">
        <li class="nav-item"><a class="nav-link" href="#about">About</a></li>
        <li class="nav-item"><a class="nav-link" href="#services">Services</a></li>
        <li class="nav-item"><a class="nav-link" href="#projects">Projects</a></li>
        <li class="nav-item"><a class="nav-link" href="#contact">Contact</a></li>
        <li class="nav-item">
    <a class="nav-link" href="https://dribbble.com" target="_blank">
      <i class="bi bi-dribbble text-danger"></i> Dribbble
    </a>
  </li>
      </ul>
    </div>
  </div>
</nav>

<!-- Hero Section -->
<section class="hero">
  <div class="hero-content container">
    <h1 class="display-4 fw-bold">Building the Future, Digitally</h1>
    <p class="lead">Custom web, app & cloud solutions to drive your business.</p>
    <a href="#contact" class="btn btn-outline-light mt-3">Let's Talk</a>
  </div>
</section>

<!-- About -->
<section id="about" class="py-5 text-center">
  <div class="container">
    <h2>About Us</h2>
    <p class="mt-3">Nammatech is a creative technology partner that delivers world-class digital products. We collaborate with clients to create experiences that transform businesses.</p>
  </div>
</section>

<!-- Services -->
<section id="services" class="py-5 bg-light">
  <div class="container text-center">
    <h2>Our Services</h2>
    <div class="row mt-4 g-4">
      <div class="col-md-4">
        <div class="card service-card shadow-sm h-100">
          <div class="card-body">
            <i class="bi bi-laptop fs-1 text-primary"></i>
            <h5 class="card-title mt-3">Web Design</h5>
            <p>Modern, responsive websites that reflect your brand.</p>
          </div>
        </div>
      </div>
      <div class="col-md-4">
        <div class="card service-card shadow-sm h-100">
          <div class="card-body">
            <i class="bi bi-phone fs-1 text-success"></i>
            <h5 class="card-title mt-3">App Development</h5>
            <p>Cross-platform mobile apps tailored for performance.</p>
          </div>
        </div>
      </div>
      <div class="col-md-4">
        <div class="card service-card shadow-sm h-100">
          <div class="card-body">
            <i class="bi bi-cloud-arrow-up fs-1 text-danger"></i>
            <h5 class="card-title mt-3">Cloud Solutions</h5>
            <p>Deploy, scale, and manage your apps with cloud technology.</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>
<!-- Gallery/Projects -->
<section id="projects" class="py-5">
  <div class="container text-center">
    <h2>Our Work</h2>
    <div class="row g-4 mt-4">
      <div class="col-md-4">
        <img src="https://static.vecteezy.com/system/resources/previews/000/523/185/original/mobile-application-development-concept-mobile-programming-coding-multi-platform-ui-ux-design-and-web-development-vector.jpg" class="gallery-img rounded" alt="">
        <div class="mt-2 d-flex justify-content-around">
          <a href="https://dribbble.com" target="_blank" class="btn btn-outline-danger btn-sm">
            <i class="bi bi-dribbble"></i> Dribbble
          </a>
          <button class="btn btn-outline-primary btn-sm">
            <i class="bi bi-hand-thumbs-up"></i> Like
          </button>
          <button class="btn btn-outline-secondary btn-sm">
            <i class="bi bi-eye"></i> View
          </button>
        </div>
      </div>
      <div class="col-md-4">
        <img src="https://static.vecteezy.com/system/resources/previews/004/946/784/original/app-development-concept-isometric-landing-page-team-create-and-optimizes-mobile-application-interface-building-process-3d-web-banner-template-illustration-with-people-scene-in-flat-design-vector.jpg" class="gallery-img rounded" alt="">
        <div class="mt-2 d-flex justify-content-around">
          <a href="https://dribbble.com" target="_blank" class="btn btn-outline-danger btn-sm">
            <i class="bi bi-dribbble"></i> Dribbble
          </a>
          <button class="btn btn-outline-primary btn-sm">
            <i class="bi bi-hand-thumbs-up"></i> Like
          </button>
          <button class="btn btn-outline-secondary btn-sm">
            <i class="bi bi-eye"></i> View
          </button>
        </div>
      </div>
      <div class="col-md-4">
        <img src="https://www.kaspersky.com/content/en-global/images/repository/isc/2020/what-is-cloud-security01.jpg" class="gallery-img rounded" alt="">
        <div class="mt-2 d-flex justify-content-around">
          <a href="https://dribbble.com" target="_blank" class="btn btn-outline-danger btn-sm">
            <i class="bi bi-dribbble"></i> Dribbble
          </a>
          <button class="btn btn-outline-primary btn-sm">
            <i class="bi bi-hand-thumbs-up"></i> Like
          </button>
          <button class="btn btn-outline-secondary btn-sm">
            <i class="bi bi-eye"></i> View
          </button>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- Testimonials -->
<section class="py-5 bg-light text-center">
  <div class="container">
    <h2>What Clients Say</h2>
    <div class="row mt-4">
      <div class="col-md-4">
        <div class="testimonial">
          <img src="https://randomuser.me/api/portraits/women/44.jpg" alt="">
          <p class="mt-2"><strong>aparna George</strong><br>“They delivered our platform on time with impressive design and functionality!”</p>
        </div>
      </div>
      <div class="col-md-4">
        <div class="testimonial">
          <img src="https://randomuser.me/api/portraits/men/35.jpg" alt="">
          <p class="mt-2"><strong>Mark Thomas</strong><br>“Fantastic team — their cloud strategy saved us huge costs!”</p>
        </div>
      </div>
      <div class="col-md-4">
        <div class="testimonial">
          <img src="https://randomuser.me/api/portraits/women/68.jpg" alt="">
          <p class="mt-2"><strong>Sophia Ray</strong><br>“Best web development team we’ve worked with!”</p>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- Contact -->
<section id="contact" class="py-5">
  <div class="container">
    <h2 class="text-center">Contact Us</h2>
    <form class="mt-4 col-md-6 mx-auto">
      <div class="mb-3">
        <input type="text" class="form-control" placeholder="Your Name" required>
      </div>
      <div class="mb-3">
        <input type="email" class="form-control" placeholder="Your Email" required>
      </div>
      <div class="mb-3">
        <textarea class="form-control" rows="4" placeholder="Your Message" required></textarea>
      </div>
      <div class="text-center">
        <button class="btn btn-dark" type="submit">Send Message</button>
      </div>
    </form>
  </div>
</section>

<!-- Footer -->
<footer class="bg-dark text-white text-center py-3">
  <p class="mb-0">&copy; 2025 Nammatech Solutions. All rights reserved.</p>
</footer>

<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
<script>
document.addEventListener('DOMContentLoaded', function() {
    // Smooth scrolling for navigation links
    const navLinks = document.querySelectorAll('a[href^="#"]');
    navLinks.forEach(link => {
        link.addEventListener('click', function(e) {
            e.preventDefault();
            const target = document.querySelector(this.getAttribute('href'));
            if (target) {
                target.scrollIntoView({ behavior: 'smooth' });
            }
        });
    });

    // Contact form submission handling
    const form = document.querySelector('form');
    form.addEventListener('submit', function(e) {
        e.preventDefault();
        alert('Thank you for your message! We will get back to you soon.');
        form.reset();
    });

    // Like button functionality
    const likeButtons = document.querySelectorAll('.btn-outline-primary');
    likeButtons.forEach(button => {
        button.addEventListener('click', function() {
            this.innerHTML = '<i class="bi bi-hand-thumbs-up-fill"></i> Liked';
            this.classList.remove('btn-outline-primary');
            this.classList.add('btn-primary');
            this.disabled = true;
        });
    });

    // View button functionality (placeholder)
    const viewButtons = document.querySelectorAll('.btn-outline-secondary');
    viewButtons.forEach(button => {
        button.addEventListener('click', function() {
            alert('Viewing project details... (This could open a modal in a full implementation)');
        });
    });

    // Add fade-in animation on scroll for sections
    const observerOptions = {
        threshold: 0.1,
        rootMargin: '0px 0px -50px 0px'
    };

    const observer = new IntersectionObserver((entries) => {
        entries.forEach(entry => {
            if (entry.isIntersecting) {
                entry.target.style.opacity = '1';
                entry.target.style.transform = 'translateY(0)';
            }
        });
    }, observerOptions);

    // Apply to sections
    const sections = document.querySelectorAll('section');
    sections.forEach(section => {
        section.style.opacity = '0';
        section.style.transform = 'translateY(20px)';
        section.style.transition = 'opacity 0.6s ease, transform 0.6s ease';
        observer.observe(section);
    });
});
</script>
</body>
</html>
```
# OUTPUT:
![WhatsApp Image 2025-12-24 at 8 53 23 AM](https://github.com/user-attachments/assets/63088479-44d3-4a45-8e95-1ce79a05f6bf)
![WhatsApp Image 2025-12-24 at 8 53 23 AM (1)](https://github.com/user-attachments/assets/026b4fe4-2d70-46be-86e8-67235de25875)
![WhatsApp Image 2025-12-24 at 8 53 23 AM (2)](https://github.com/user-attachments/assets/09837142-7218-4a2d-a349-2873ea7969ce)


# RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
