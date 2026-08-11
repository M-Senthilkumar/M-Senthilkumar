<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>✨ GitHub Profile README · preview</title>
    <!-- Font Awesome 6 (free icons) -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background: #0d1117;
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            font-family: 'Segoe UI', 'Helvetica Neue', system-ui, -apple-system, sans-serif;
            padding: 1.5rem;
        }

        /* main card – exactly like a polished GitHub README card */
        .github-readme {
            max-width: 840px;
            width: 100%;
            background: #0d1117;
            border-radius: 32px;
            padding: 2.2rem 2.5rem;
            border: 1px solid #30363d;
            box-shadow: 0 20px 40px -12px rgba(0,0,0,0.9), 0 0 0 1px rgba(255,255,255,0.02);
            transition: all 0.2s;
        }

        /* header: avatar + title */
        .profile-head {
            display: flex;
            align-items: center;
            gap: 1.2rem;
            flex-wrap: wrap;
            margin-bottom: 2rem;
            padding-bottom: 1.6rem;
            border-bottom: 1px solid #21262d;
        }

        .avatar-icon {
            background: linear-gradient(145deg, #f0883e, #f6a85b);
            width: 76px;
            height: 76px;
            border-radius: 40px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 2.6rem;
            color: #0d1117;
            box-shadow: 0 6px 14px rgba(0,0,0,0.5);
            flex-shrink: 0;
        }

        .title-block h1 {
            color: #f0f6fc;
            font-weight: 700;
            font-size: 2.2rem;
            letter-spacing: -0.3px;
            display: flex;
            align-items: center;
            flex-wrap: wrap;
            gap: 0.4rem;
        }

        .title-block h1 i {
            color: #58a6ff;
            font-size: 1.8rem;
        }

        .badge-pro {
            background: #1f6feb;
            color: white;
            font-size: 0.65rem;
            font-weight: 700;
            padding: 0.2rem 0.9rem;
            border-radius: 30px;
            letter-spacing: 0.3px;
            display: inline-block;
            box-shadow: 0 2px 8px rgba(31,111,235,0.3);
        }

        .subhead {
            color: #8b949e;
            font-size: 0.95rem;
            margin-top: 0.2rem;
            display: flex;
            flex-wrap: wrap;
            gap: 0.3rem 0.8rem;
        }

        .subhead i {
            color: #58a6ff;
            width: 1.2rem;
        }

        /* quote / tagline */
        .quote-box {
            background: #161b22;
            padding: 1rem 1.6rem;
            border-radius: 20px;
            border-left: 6px solid #f0883e;
            margin-bottom: 2rem;
            display: flex;
            align-items: center;
            gap: 0.8rem;
            border: 1px solid #30363d;
            border-left-width: 6px;
            color: #c9d1d9;
            font-style: italic;
        }

        .quote-box i {
            color: #f6a85b;
            font-size: 1.3rem;
        }

        .quote-box .hl {
            color: #f6a85b;
            font-style: normal;
            font-weight: 500;
        }

        /* stats grid */
        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
            gap: 1rem;
            margin-bottom: 2rem;
        }

        .stat-card {
            background: #161b22;
            border-radius: 20px;
            padding: 0.9rem 0.4rem;
            text-align: center;
            border: 1px solid #30363d;
            box-shadow: 0 4px 8px rgba(0,0,0,0.3);
            transition: 0.15s ease;
        }

        .stat-card:hover {
            border-color: #58a6ff;
            transform: translateY(-3px);
        }

        .stat-number {
            font-size: 1.9rem;
            font-weight: 700;
            color: #f0f6fc;
            display: block;
            line-height: 1.2;
        }

        .stat-label {
            color: #8b949e;
            font-size: 0.7rem;
            text-transform: uppercase;
            letter-spacing: 0.3px;
            margin-top: 2px;
        }

        .stat-icon {
            color: #58a6ff;
            margin-right: 0.2rem;
        }

        /* tech & tools */
        .tech-wrapper {
            background: #0d1117;
            border-radius: 20px;
            padding: 0.6rem 0.2rem 0.2rem 0.2rem;
            margin-bottom: 1.8rem;
            border-top: 1px solid #21262d;
        }

        .tech-title {
            color: #f0f6fc;
            font-weight: 600;
            font-size: 1rem;
            margin-bottom: 1rem;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

        .tech-title i {
            color: #f6a85b;
        }

        .tech-pills {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 0.7rem 1.2rem;
        }

        .tech-pills span {
            background: #161b22;
            padding: 0.4rem 1.1rem;
            border-radius: 40px;
            font-size: 0.85rem;
            font-weight: 500;
            color: #c9d1d9;
            border: 1px solid #30363d;
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
            transition: 0.1s ease;
            box-shadow: 0 2px 4px rgba(0,0,0,0.2);
        }

        .tech-pills span i {
            color: #f6a85b;
            font-size: 0.95rem;
        }

        .tech-pills span:hover {
            background: #1f6feb20;
            border-color: #58a6ff;
            color: #f0f6fc;
        }

        /* social links */
        .social-bar {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 1.2rem 2rem;
            background: #161b22;
            padding: 1rem 1.8rem;
            border-radius: 40px;
            border: 1px solid #30363d;
            margin-top: 1.2rem;
        }

        .social-bar a {
            color: #8b949e;
            font-size: 1.1rem;
            text-decoration: none;
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
            font-weight: 500;
            transition: 0.15s;
        }

        .social-bar a i {
            font-size: 1.4rem;
            width: 1.6rem;
            text-align: center;
        }

        .social-bar a:hover {
            color: #f0f6fc;
            transform: translateY(-2px);
        }

        .social-bar a .handle {
            font-size: 0.8rem;
            font-weight: 400;
            color: #8b949e;
        }

        /* footer */
        .footer-note {
            margin-top: 2rem;
            text-align: center;
            font-size: 0.7rem;
            color: #484f58;
            border-top: 1px solid #21262d;
            padding-top: 1rem;
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 1.2rem;
        }

        .footer-note i {
            color: #f6a85b;
        }

        .copy-hint {
            margin-top: 0.8rem;
            text-align: right;
            font-size: 0.7rem;
            color: #30363d;
            border-top: 1px dashed #21262d;
            padding-top: 0.8rem;
        }

        .copy-hint i {
            color: #58a6ff;
        }

        /* responsive */
        @media (max-width: 600px) {
            .github-readme {
                padding: 1.5rem;
            }
            .profile-head {
                flex-direction: column;
                align-items: flex-start;
            }
            .title-block h1 {
                font-size: 1.8rem;
            }
            .stats-grid {
                grid-template-columns: 1fr 1fr;
            }
        }
    </style>
</head>
<body>
<div class="github-readme">

    <!-- HEADER -->
    <div class="profile-head">
        <div class="avatar-icon">
            <i class="fas fa-code"></i>
        </div>
        <div class="title-block">
            <h1>
                <i class="fas fa-at"></i> your-username
                <span class="badge-pro"><i class="fas fa-check-circle" style="margin-right: 4px;"></i>PRO</span>
            </h1>
            <div class="subhead">
                <span><i class="fas fa-map-pin"></i> Bangalore, India</span>
                <span><i class="fas fa-briefcase"></i> Full-stack · 5+ yrs</span>
                <span><i class="fas fa-graduation-cap"></i> B.E. CSE</span>
            </div>
        </div>
    </div>

    <!-- QUOTE -->
    <div class="quote-box">
        <i class="fas fa-quote-left"></i>
        <span>“Crafting <span class="hl">clean</span>, <span class="hl">scalable</span> solutions · 
        <i class="fas fa-heart" style="color: #f6a85b; margin: 0 3px;"></i> open source”</span>
    </div>

    <!-- STATS -->
    <div class="stats-grid">
        <div class="stat-card">
            <span class="stat-number"><i class="fas fa-star stat-icon"></i> 1.4k</span>
            <span class="stat-label">Stars</span>
        </div>
        <div class="stat-card">
            <span class="stat-number"><i class="fas fa-code-branch stat-icon"></i> 92</span>
            <span class="stat-label">Repos</span>
        </div>
        <div class="stat-card">
            <span class="stat-number"><i class="fas fa-users stat-icon"></i> 410</span>
            <span class="stat-label">Followers</span>
        </div>
        <div class="stat-card">
            <span class="stat-number"><i class="fas fa-trophy stat-icon"></i> 22</span>
            <span class="stat-label">Contributions</span>
        </div>
    </div>

    <!-- TECH STACK -->
    <div class="tech-wrapper">
        <div class="tech-title">
            <i class="fas fa-cog"></i>  Stack & tools
        </div>
        <div class="tech-pills">
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

    <!-- SOCIAL LINKS -->
    <div class="social-bar">
        <a href="#"><i class="fab fa-github"></i> <span class="handle">@your-username</span></a>
        <a href="#"><i class="fab fa-twitter"></i> <span class="handle">@your-twitter</span></a>
        <a href="#"><i class="fab fa-linkedin-in"></i> <span class="handle">in/your-profile</span></a>
        <a href="#"><i class="fas fa-envelope"></i> <span class="handle">work@email.dev</span></a>
    </div>

    <!-- FOOTER -->
    <div class="footer-note">
        <span><i class="fas fa-code"></i> 2026 · built with <i class="fas fa-heart" style="color: #f6a85b;"></i></span>
        <span><i class="fas fa-flag-checkered"></i> always building</span>
        <span><i class="fas fa-mug-hot"></i>  ☕ coffee-driven</span>
    </div>

    <!-- small hint: ready to copy/paste -->
    <div class="copy-hint">
        <i class="fas fa-edit"></i>  copy this code into your <span style="background: #161b22; padding: 0.1rem 0.6rem; border-radius: 12px; font-family: monospace;">README.md</span> 
        <i class="fas fa-arrow-right" style="margin-left: 6px; color: #58a6ff;"></i>
    </div>

</div>
</body>
</html>
