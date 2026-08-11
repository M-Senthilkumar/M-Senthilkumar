<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>✨ Attractive GitHub Profile README</title>
  <!-- Font Awesome Icons (free) -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
  <style>
    /* modern, clean, and colorful style */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      background: linear-gradient(145deg, #0d1117 0%, #161b22 100%);
      min-height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      font-family: 'Segoe UI', system-ui, -apple-system, BlinkMacSystemFont, 'Helvetica Neue', sans-serif;
      padding: 1.5rem;
    }

    /* card container – simulates a GitHub profile README “card” */
    .readme-card {
      max-width: 820px;
      width: 100%;
      background: #0d1117;
      border-radius: 32px;
      padding: 2.2rem 2.5rem;
      box-shadow: 0 20px 40px -12px rgba(0, 0, 0, 0.8), 0 0 0 1px rgba(255, 255, 255, 0.03);
      border: 1px solid #30363d;
      transition: all 0.2s ease;
    }

    /* header / avatar + title */
    .profile-header {
      display: flex;
      align-items: center;
      gap: 1.2rem;
      flex-wrap: wrap;
      margin-bottom: 2rem;
      border-bottom: 1px solid #21262d;
      padding-bottom: 1.8rem;
    }

    .avatar {
      background: linear-gradient(135deg, #f0883e, #f6a85b);
      width: 80px;
      height: 80px;
      border-radius: 40px;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 2.8rem;
      color: #0d1117;
      box-shadow: 0 6px 12px rgba(0, 0, 0, 0.6);
      flex-shrink: 0;
    }

    .title-group h1 {
      color: #f0f6fc;
      font-weight: 700;
      font-size: 2.1rem;
      letter-spacing: -0.5px;
      margin-bottom: 0.2rem;
    }

    .title-group .badge {
      background: #238636;
      color: white;
      font-size: 0.7rem;
      font-weight: 600;
      padding: 0.2rem 0.8rem;
      border-radius: 20px;
      display: inline-block;
      text-transform: uppercase;
      letter-spacing: 0.3px;
      background: #1f6feb;
      box-shadow: 0 2px 6px rgba(31, 111, 235, 0.3);
      margin-left: 0.5rem;
    }

    .title-group .subhead {
      color: #8b949e;
      font-size: 0.95rem;
      margin-top: 0.2rem;
      display: flex;
      align-items: center;
      gap: 0.3rem;
      flex-wrap: wrap;
    }

    .subhead i {
      color: #58a6ff;
    }

    /* tagline / quote */
    .quote-section {
      background: #161b22;
      padding: 1.2rem 1.6rem;
      border-radius: 20px;
      border-left: 4px solid #f0883e;
      margin-bottom: 2rem;
      color: #c9d1d9;
      font-style: italic;
      display: flex;
      align-items: center;
      gap: 0.8rem;
      border: 1px solid #30363d;
      border-left-width: 6px;
    }

    .quote-section i {
      color: #f6a85b;
      font-size: 1.4rem;
    }

    .quote-section span {
      font-weight: 400;
      letter-spacing: 0.2px;
    }

    .quote-section .highlight {
      color: #f6a85b;
      font-weight: 500;
      font-style: normal;
    }

    /* stats grid — like GitHub stats cards */
    .stats-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
      gap: 1.2rem;
      margin-bottom: 2.2rem;
    }

    .stat-item {
      background: #161b22;
      border-radius: 20px;
      padding: 0.9rem 0.6rem;
      text-align: center;
      border: 1px solid #30363d;
      transition: transform 0.15s ease, border-color 0.2s;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
    }

    .stat-item:hover {
      transform: translateY(-3px);
      border-color: #58a6ff;
    }

    .stat-number {
      font-size: 1.8rem;
      font-weight: 700;
      color: #f0f6fc;
      display: block;
      line-height: 1.2;
    }

    .stat-label {
      color: #8b949e;
      font-size: 0.75rem;
      text-transform: uppercase;
      letter-spacing: 0.3px;
      margin-top: 2px;
    }

    .stat-icon {
      color: #58a6ff;
      margin-right: 0.2rem;
    }

    /* tech / tools section */
    .tech-section {
      background: #0d1117;
      border-radius: 20px;
      padding: 1.2rem 0.8rem 0.8rem 0.8rem;
      margin-bottom: 2rem;
      border-top: 1px solid #21262d;
    }

    .tech-title {
      color: #f0f6fc;
      font-weight: 600;
      font-size: 1rem;
      letter-spacing: 0.5px;
      margin-bottom: 1rem;
      display: flex;
      align-items: center;
      gap: 0.6rem;
    }

    .tech-title i {
      color: #f6a85b;
    }

    .tech-icons {
      display: flex;
      flex-wrap: wrap;
      gap: 0.9rem 1.6rem;
      justify-content: center;
    }

    .tech-icons span {
      background: #161b22;
      padding: 0.4rem 1rem;
      border-radius: 40px;
      font-size: 0.85rem;
      font-weight: 500;
      color: #c9d1d9;
      border: 1px solid #30363d;
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      transition: all 0.15s;
      box-shadow: 0 2px 4px rgba(0,0,0,0.3);
    }

    .tech-icons span i {
      color: #f6a85b;
      font-size: 1rem;
    }

    .tech-icons span:hover {
      background: #1f6feb20;
      border-color: #58a6ff;
      color: #f0f6fc;
      transform: scale(1.02);
    }

    /* activity / social links */
    .social-links {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 1.2rem 2rem;
      background: #161b22;
      padding: 1.2rem 1.5rem;
      border-radius: 40px;
      border: 1px solid #30363d;
      margin-top: 1.5rem;
    }

    .social-links a {
      color: #8b949e;
      font-size: 1.2rem;
      transition: all 0.15s;
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      text-decoration: none;
      font-weight: 500;
    }

    .social-links a i {
      font-size: 1.4rem;
      width: 1.6rem;
      text-align: center;
    }

    .social-links a:hover {
      color: #f0f6fc;
      transform: translateY(-2px);
    }

    .social-links a .handle {
      font-size: 0.8rem;
      font-weight: 400;
      color: #8b949e;
    }

    .footer-note {
      margin-top: 2rem;
      text-align: center;
      font-size: 0.75rem;
      color: #484f58;
      letter-spacing: 0.5px;
      border-top: 1px solid #21262d;
      padding-top: 1.2rem;
      display: flex;
      justify-content: center;
      gap: 1.2rem;
      flex-wrap: wrap;
    }

    .footer-note i {
      color: #f6a85b;
      margin: 0 0.2rem;
    }

    /* responsive */
    @media (max-width: 600px) {
      .readme-card {
        padding: 1.5rem;
      }
      .profile-header {
        flex-direction: column;
        align-items: flex-start;
      }
      .title-group h1 {
        font-size: 1.8rem;
      }
      .stats-grid {
        grid-template-columns: 1fr 1fr;
      }
    }
  </style>
</head>
<body>
  <div class="readme-card">
    <!-- header with avatar and title -->
    <div class="profile-header">
      <div class="avatar">
        <i class="fas fa-code"></i>
      </div>
      <div class="title-group">
        <h1>
          <i class="fas fa-at" style="color: #58a6ff; font-size: 1.6rem; margin-right: 4px;"></i>
          your-username
          <span class="badge"><i class="fas fa-check-circle" style="margin-right: 4px;"></i>PRO</span>
        </h1>
        <div class="subhead">
          <i class="fas fa-map-pin"></i> 
          <span>📍 Bangalore, India</span>
          <span style="margin: 0 4px;">•</span>
          <i class="fas fa-briefcase"></i> 
          <span>Full-stack developer · 5+ yrs</span>
        </div>
      </div>
    </div>

    <!-- quote / tagline -->
    <div class="quote-section">
      <i class="fas fa-quote-left"></i>
      <span>
        “Building <span class="highlight">clean</span>, <span class="highlight">scalable</span> apps with a 
        <i class="fas fa-heart" style="color: #f6a85b; margin: 0 2px;"></i> for open source.”
      </span>
    </div>

    <!-- stats like GitHub profile stats -->
    <div class="stats-grid">
      <div class="stat-item">
        <span class="stat-number"><i class="fas fa-star stat-icon"></i> 1.2k</span>
        <span class="stat-label">Stars earned</span>
      </div>
      <div class="stat-item">
        <span class="stat-number"><i class="fas fa-code-branch stat-icon"></i> 84</span>
        <span class="stat-label">Repositories</span>
      </div>
      <div class="stat-item">
        <span class="stat-number"><i class="fas fa-users stat-icon"></i> 320</span>
        <span class="stat-label">Followers</span>
      </div>
      <div class="stat-item">
        <span class="stat-number"><i class="fas fa-trophy stat-icon"></i> 14</span>
        <span class="stat-label">Contributions</span>
      </div>
    </div>

    <!-- tech stack with icons (Font Awesome) -->
    <div class="tech-section">
      <div class="tech-title">
        <i class="fas fa-cog"></i>  Tech stack & tools
      </div>
      <div class="tech-icons">
        <span><i class="fab fa-js-square"></i> JavaScript</span>
        <span><i class="fab fa-react"></i> React</span>
        <span><i class="fab fa-node"></i> Node.js</span>
        <span><i class="fab fa-python"></i> Python</span>
        <span><i class="fas fa-database"></i> MongoDB</span>
        <span><i class="fab fa-docker"></i> Docker</span>
        <span><i class="fab fa-git-alt"></i> Git</span>
        <span><i class="fas fa-cloud"></i> AWS</span>
      </div>
    </div>

    <!-- social / contact links (attractive) -->
    <div class="social-links">
      <a href="#"><i class="fab fa-github"></i> <span class="handle">@your-username</span></a>
      <a href="#"><i class="fab fa-twitter"></i> <span class="handle">@your-twitter</span></a>
      <a href="#"><i class="fab fa-linkedin-in"></i> <span class="handle">in/your-profile</span></a>
      <a href="#"><i class="fas fa-envelope"></i> <span class="handle">work@email.dev</span></a>
    </div>

    <!-- footer / extra info -->
    <div class="footer-note">
      <span><i class="fas fa-code"></i> 2026 · crafted with <i class="fas fa-heart" style="color: #f6a85b;"></i></span>
      <span><i class="fas fa-flag-checkered"></i> always building</span>
      <span><i class="fas fa-mug-hot"></i>  ☕ powered by coffee</span>
    </div>

    <!-- small hint: this is a README preview -->
    <div style="margin-top: 0.8rem; text-align: right; font-size: 0.7rem; color: #30363d; border-top: 1px dashed #21262d; padding-top: 0.8rem;">
      <i class="fas fa-edit"></i>  edit this card to make it yours — copy the code inside 
      <span style="background: #161b22; padding: 0.1rem 0.6rem; border-radius: 12px; font-family: monospace;">README.md</span>
    </div>
  </div>
</body>
</html>
