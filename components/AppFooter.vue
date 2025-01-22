<template>
    <footer class="footer">
        <div class="footer-content">
            <!-- Left Section: Social Media Links -->
        <div class="footer-social">
            <h2 class="footer-heading">Stay Connected</h2>
            <div class="social-icons">
            <li><a href="#" aria-label="Facebook">Facebook</a></li>
            <li><a href="#" aria-label="Twitter">Twitter</a></li>
            <li><a href="#" aria-label="Instagram">Instagrazm</a></li>
          </div>
        </div>
  
        <!-- Right Section: Additional Information -->
        <div class="footer-info">
          <ul class="footer-links">
            <li><a href="#privacy">Privacy Policy</a></li>
            <li><a href="#terms">Terms of Service</a></li>
            <li><a href="#contact">Contact Us</a></li>
          </ul>
        </div>
        <br />
    </div>
    <p>© 2025 Your Website Name. All rights reserved.</p>
    </footer>
  </template>
  
  <script>
  export default {
    name: "FooterComponent",
  };
  </script>
  
  <style scoped>
  :root {
    --footer-font-family: Arial, sans-serif;
    --footer-bg-color: #f4f4f9;
    --footer-primary-text-color: #2c3e50;
    --footer-secondary-text-color: #34495e;
    --footer-link-color: #2980b9;
    --footer-link-hover-color: #16a085;
    --footer-note-color: #7f8c8d;
    --footer-border-color: #2980b9;
    --footer-padding: 40px;
    --footer-link-spacing: 15px;
    --footer-font-size: 1rem;
    --footer-heading-size: 1.2rem;
  }
  
  .footer {
    background-color: var(--footer-bg-color);
    padding: var(--footer-padding);
    text-align: center;
    color: var(--footer-secondary-text-color);
    border-top: 2px solid var(--footer-border-color);
    box-shadow: 0 -4px 6px rgba(0, 0, 0, 0.1);
  }
  
  .footer-content {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    flex-wrap: wrap;
  }
  
  .footer-social,
  .footer-info {
    flex: 1;
    margin: 10px;
  }
  
  .footer-heading {
    margin: 0 0 15px;
    font-size: var(--footer-heading-size);
    font-weight: bold;
    color: var(--footer-primary-text-color);
    text-align: center;
  }
  
  .footer-links {
    list-style: none;
    padding: 0;
    margin: 20px 0;
  }
  
  .footer-links li {
    margin: 0;
  }
  
  .footer-links li a {
    text-decoration: none;
    color: var(--footer-link-color);
    font-size: var(--footer-font-size);
    font-weight: 600;
    transition: color 0.3s ease;
  }
  
  .footer-links li a:hover {
    color: var(--footer-link-hover-color);
  }
  
  .social-icons {
    margin-top: 20px;
    display: flex;
    gap: 10px;
  }
  
  .social-icons a {
    text-decoration: none;
    font-size: 1.2rem;
    color: var(--footer-link-color);
    transition: color 0.3s ease;
  }
  
  .social-icons a:hover {
    color: var(--footer-primary-text-color);
  }
  
  .footer p {
    margin: 10px 0;
    font-size: var(--footer-font-size);
    color: var(--footer-note-color);
  }
  </style>
  