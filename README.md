Mohammed Mustaqeem Uddin - Interactive Profile
<div align="center">
<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

.profile-container {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    border-radius: 20px;
    padding: 2rem;
    margin: 2rem 0;
    position: relative;
    overflow: hidden;
}

.stars {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    pointer-events: none;
}

.star {
    position: absolute;
    width: 2px;
    height: 2px;
    background: white;
    border-radius: 50%;
    animation: twinkle 2s infinite alternate;
}

@keyframes twinkle {
    0% { opacity: 0.3; }
    100% { opacity: 1; }
}

.profile-card {
    background: rgba(255, 255, 255, 0.95);
    backdrop-filter: blur(20px);
    border-radius: 30px;
    padding: 3rem;
    text-align: center;
    box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
    border: 1px solid rgba(255, 255, 255, 0.3);
    transform: translateY(20px);
    animation: slideIn 1s ease-out forwards;
    margin-bottom: 2rem;
    position: relative;
    z-index: 1;
}

@keyframes slideIn {
    to {
        transform: translateY(0);
        opacity: 1;
    }
}

.profile-avatar {
    width: 150px;
    height: 150px;
    border-radius: 50%;
    background: linear-gradient(45deg, #667eea, #764ba2);
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 0 auto 2rem;
    font-size: 4rem;
    color: white;
    animation: float 3s ease-in-out infinite;
    position: relative;
    overflow: hidden;
}

.profile-avatar::before {
    content: '';
    position: absolute;
    top: -50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: linear-gradient(45deg, transparent, rgba(255,255,255,0.3), transparent);
    animation: shine 2s infinite;
}

@keyframes float {
    0%, 100% { transform: translateY(0px); }
    50% { transform: translateY(-10px); }
}

@keyframes shine {
    0% { transform: rotate(0deg); }
    100% { transform: rotate(360deg); }
}

.gradient-title {
    font-size: 3rem;
    background: linear-gradient(45deg, #667eea, #764ba2);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 1rem;
    animation: fadeInUp 1s 0.3s both;
}

.subtitle {
    font-size: 1.3rem;
    color: #555;
    margin-bottom: 1rem;
    animation: fadeInUp 1s 0.6s both;
}

.description {
    font-size: 1.1rem;
    color: #666;
    line-height: 1.6;
    margin-bottom: 2rem;
    animation: fadeInUp 1s 0.9s both;
}

@keyframes fadeInUp {
    from {
        opacity: 0;
        transform: translateY(30px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

.section {
    background: rgba(255, 255, 255, 0.95);
    backdrop-filter: blur(20px);
    border-radius: 20px;
    padding: 2rem;
    margin-bottom: 2rem;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
    border: 1px solid rgba(255, 255, 255, 0.3);
    transform: translateY(20px);
    opacity: 0;
    animation: slideIn 1s ease-out forwards;
    position: relative;
    z-index: 1;
    transition: all 0.3s ease;
}

.section:hover {
    transform: translateY(-5px);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.3);
}

.section:nth-child(2) { animation-delay: 0.3s; }
.section:nth-child(3) { animation-delay: 0.6s; }

.section-title {
    font-size: 1.8rem;
    color: #333;
    margin-bottom: 1.5rem;
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 0.5rem;
}

.social-links {
    display: flex;
    justify-content: center;
    gap: 1rem;
    flex-wrap: wrap;
}

.social-btn {
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    padding: 0.8rem 1.5rem;
    border-radius: 25px;
    text-decoration: none;
    color: white;
    font-weight: 600;
    transition: all 0.3s ease;
    position: relative;
    overflow: hidden;
}

.social-btn::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(255,255,255,0.3), transparent);
    transition: left 0.5s;
}

.social-btn:hover::before {
    left: 100%;
}

.social-btn:hover {
    transform: translateY(-2px);
    box-shadow: 0 10px 25px rgba(0, 0, 0, 0.3);
}

.instagram { background: linear-gradient(45deg, #f09433 0%,#e6683c 25%,#dc2743 50%,#cc2366 75%,#bc1888 100%); }
.linkedin { background: #0077B5; }
.twitter { background: #000000; }
.email { background: #D14836; }

.tech-stack {
    display: flex;
    justify-content: center;
    gap: 1rem;
    flex-wrap: wrap;
}

.tech-badge {
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    padding: 1rem 1.5rem;
    border-radius: 15px;
    color: white;
    font-weight: 600;
    text-decoration: none;
    transition: all 0.3s ease;
    position: relative;
    overflow: hidden;
}

.tech-badge::after {
    content: '';
    position: absolute;
    top: 50%;
    left: 50%;
    width: 0;
    height: 0;
    background: rgba(255, 255, 255, 0.2);
    border-radius: 50%;
    transition: all 0.4s ease;
    transform: translate(-50%, -50%);
}

.tech-badge:hover::after {
    width: 300px;
    height: 300px;
}

.tech-badge:hover {
    transform: scale(1.05);
}

.python { background: linear-gradient(45deg, #3670A0, #ffdd54); }
.mysql { background: #4479A1; }

.emoji {
    font-size: 1.5rem;
    display: inline-block;
    animation: bounce 2s infinite;
}

@keyframes bounce {
    0%, 20%, 50%, 80%, 100% { transform: translateY(0); }
    40% { transform: translateY(-10px); }
    60% { transform: translateY(-5px); }
}

.floating-shapes {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    pointer-events: none;
}

.shape {
    position: absolute;
    border-radius: 50%;
    background: rgba(255, 255, 255, 0.1);
    animation: float-shapes 10s infinite linear;
}

@keyframes float-shapes {
    0% { transform: translateY(100%) rotate(0deg); }
    100% { transform: translateY(-100px) rotate(360deg); }
}

@media (max-width: 768px) {
    .gradient-title { font-size: 2rem; }
    .subtitle { font-size: 1.1rem; }
    .social-links { flex-direction: column; align-items: center; }
    .tech-stack { flex-direction: column; align-items: center; }
    .profile-card { padding: 2rem; }
}
</style>
<div class="profile-container">
    <div class="stars" id="stars"></div>
    <div class="floating-shapes" id="floating-shapes"></div>
<div class="profile-card">
    <div class="profile-avatar">
        👨‍💻
    </div>
    <h1 class="gradient-title">Hi <span class="emoji">👋</span>, I'm Mohammed Mustaqeem Uddin</h1>
    <div class="subtitle">
        <span class="emoji">🚀</span> Aspiring Data Scientist | Curious Learner | Passionate About Turning Data into Insight
    </div>
    <p class="description">
        Exploring the world of data with curiosity as my fuel — passionately pursuing patterns, insights, and real-world impact.
    </p>
</div>

<div class="section">
    <h2 class="section-title">
        <span class="emoji">🌐</span> Connect with Me
    </h2>
    <div class="social-links">
        <a href="https://instagram.com/mustaqeem._7" target="_blank" class="social-btn instagram">
            📸 Instagram
        </a>
        <a href="https://linkedin.com/in/mohammed-mustaqeem-uddin" target="_blank" class="social-btn linkedin">
            💼 LinkedIn
        </a>
        <a href="https://x.com/mohammed_u24604" target="_blank" class="social-btn twitter">
            🐦 X (Twitter)
        </a>
        <a href="mailto:mustaqeemu17@gmail.com" target="_blank" class="social-btn email">
            ✉️ Email
        </a>
    </div>
</div>

<div class="section">
    <h2 class="section-title">
        <span class="emoji">💻</span> Tech Stack
    </h2>
    <div class="tech-stack">
        <div class="tech-badge python">
            🐍 Python
        </div>
        <div class="tech-badge mysql">
            🗄️ MySQL
        </div>
    </div>
</div>
</div>
<script>
// Create floating stars
function createStars() {
    const starsContainer = document.getElementById('stars');
    for (let i = 0; i < 50; i++) {
        const star = document.createElement('div');
        star.className = 'star';
        star.style.left = Math.random() * 100 + '%';
        star.style.top = Math.random() * 100 + '%';
        star.style.animationDelay = Math.random() * 2 + 's';
        starsContainer.appendChild(star);
    }
}

// Create floating shapes
function createFloatingShapes() {
    const shapesContainer = document.getElementById('floating-shapes');
    for (let i = 0; i < 10; i++) {
        const shape = document.createElement('div');
        shape.className = 'shape';
        shape.style.left = Math.random() * 100 + '%';
        shape.style.width = shape.style.height = (Math.random() * 30 + 10) + 'px';
        shape.style.animationDuration = (Math.random() * 10 + 10) + 's';
        shape.style.animationDelay = Math.random() * 5 + 's';
        shapesContainer.appendChild(shape);
    }
}

// Initialize animations when page loads
document.addEventListener('DOMContentLoaded', function() {
    createStars();
    createFloatingShapes();
});
</script>
</div>

📊 GitHub Stats
<div align="center">
Show Image
Show Image
Show Image
</div>

🏆 GitHub Trophies
<div align="center">
Show Image
</div>

🎯 Current Focus

🔭 Working on Data Science Projects
🌱 Learning Machine Learning & AI
👯 Looking to collaborate on Open Source Data Projects
💬 Ask me about Python, Data Analysis, MySQL
⚡ Fun fact: I turn coffee into code and data into insights!


<div align="center">
💫 "Data is the new oil, but insights are the refined fuel that powers decisions!"
Show Image

Thanks for visiting my profile! Let's connect and build something amazing together! 🚀
</div>
