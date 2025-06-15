<template>
    <section class="contact-section" data-aos="fade-up">
      <h2 class="contact-title">
        <span class="highlight">Let's</span> Work <span class="highlight">Together</span>
      </h2>
  
      <div class="contact-grid">
        <!-- Left Info -->
        <div class="contact-info">
          <h3 class="contact-subheading">Ready to elevate your business?</h3>
          <p class="contact-description">
            I'm always excited to work on new projects and help businesses achieve their goals through exceptional web development.
            Let's discuss how I can help bring your vision to life.
          </p>
  
          <div class="contact-method">
            <div class="icon email-icon">📧</div>
            <div>
              <p class="label">Email</p>
              <p class="value">sakih69@outlook.com</p>
            </div>
          </div>
  
          <div class="contact-method">
            <div class="icon phone-icon">📞</div>
            <div>
              <p class="label">Phone</p>
              <p class="value">+233 54 270-1272</p>
            </div>
          </div>
        </div>
  
        <!-- Right Form -->
        <form class="contact-form">
          <label>
            <span>Name</span>
            <input type="text" placeholder="Your Name" />
          </label>
          <label>
            <span>Email</span>
            <input type="email" placeholder="your@email.com" />
          </label>
          <label>
            <span>Project Budget</span>
            <select>
              <option>$300 - $500</option>
              <option>$500 - $1,000</option>
              <option>$1,000 - $5,000 </option>
            </select>
          </label>
          <button type="submit">Send Message</button>
        </form>
      </div>
    </section>
  </template>
  
  <script>
  export default {
    name: 'Contact',
  };
  </script>
  
  <style scoped>
  .contact-section {
    padding: 4rem 1.5rem;
    max-width: 1200px;
    margin: auto;
  }
  
  .contact-title {
  font-size: 2.5rem;
  text-align: center;
  margin-bottom: 3rem;
  background: linear-gradient(to right, #ff6b6b, #48c6ef);
  background-clip: text;                /* ✅ Add this */
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

  
  .contact-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 2rem;
    flex-wrap: wrap;
  }
  
  .contact-info {
    display: flex;
    flex-direction: column;
    gap: 1.5rem;
  }
  
  .contact-subheading {
    color: #ffd700;
    font-size: 1.25rem;
    font-weight: bold;
  }
  
  .contact-description {
    color: #ccc;
    font-size: 0.95rem;
  }
  
  .contact-method {
    display: flex;
    align-items: center;
    gap: 1rem;
  }
  
  .icon {
    font-size: 1.5rem;
    padding: 0.75rem;
    border-radius: 50%;
    display: inline-flex;
    align-items: center;
    justify-content: center;
    color: white;
  }
  
  .email-icon {
    background-color: #ff5722;
  }
  
  .phone-icon {
    background-color: #00bcd4;
  }
  
  .label {
    font-weight: bold;
    font-size: 0.9rem;
    color: #fff;
  }
  
  .value {
    font-size: 0.85rem;
    color: #bbb;
  }
  
  .contact-form {
    background-color: #1e1e1e;
    border-radius: 12px;
    padding: 2rem;
    box-shadow: 0 10px 25px rgba(0, 0, 0, 0.3);
    display: flex;
    flex-direction: column;
    gap: 1.25rem;
  }
  
  .contact-form label {
    display: flex;
    flex-direction: column;
    gap: 0.25rem;
    color: #ffcc00;
    font-size: 0.9rem;
  }
  
  .contact-form input,
  .contact-form select {
    padding: 0.75rem;
    border: none;
    border-radius: 8px;
    background: #333;
    color: white;
  }
  
  .contact-form button {
    padding: 0.75rem 1rem;
    background-color: #ff6b6b;
    border: none;
    border-radius: 8px;
    color: white;
    font-weight: bold;
    cursor: pointer;
    transition: background 0.3s ease;
  }
  
  .contact-form button:hover {
    background-color: #ff5252;
  }
  
  @media (max-width: 768px) {
    .contact-grid {
      grid-template-columns: 1fr;
    }
  }
  </style>
  