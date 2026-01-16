<div style="
    font-family: 'Courier New', monospace;
    text-align: center;
    background: linear-gradient(45deg, #0f2027, #203a43, #2c5364);
    background-size: 400% 400%;
    animation: gradientBG 15s ease infinite;
    color: #fff;
    padding: 50px 20px;
    border-radius: 10px;
    position: relative;
    overflow: hidden;
">
    <style>
        @keyframes gradientBG {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        @keyframes wave {
            0% { transform: translateX(0); }
            100% { transform: translateX(-50%); }
        }
        .wave-container {
            position: absolute;
            top: 50%;
            left: 0;
            width: 200%;
            height: 200%;
            background: rgba(255, 255, 255, 0.05);
            transform: translateY(-50%);
            z-index: 0;
        }
        .wave {
            position: absolute;
            top: -100%;
            left: 0;
            width: 100%;
            height: 100%;
            background: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320"><path fill="rgba(0, 255, 255, 0.2)" fill-opacity="1" d="M0,192L48,197.3C96,203,192,213,288,229.3C384,245,480,267,576,250.7C672,235,768,181,864,160C960,139,1056,149,1152,160C1248,171,1344,181,1392,186.7L1440,192L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z"></path></svg>');
            background-size: 50% 100%;
            animation: wave 20s linear infinite;
        }
        .wave:nth-child(2) {
            top: -105%;
            animation: wave 15s linear infinite reverse;
            opacity: 0.5;
        }
        @keyframes typing {
            from { width: 0 }
            to { width: 100% }
        }
        @keyframes blink-caret {
            from, to { border-color: transparent }
            50% { border-color: orange; }
        }
        .typing-text {
            overflow: hidden;
            border-right: .15em solid orange;
            white-space: nowrap;
            margin: 0 auto;
            letter-spacing: .15em;
            animation: 
                typing 3.5s steps(40, end),
                blink-caret .75s step-end infinite;
            display: inline-block;
        }
    </style>
    <div class="wave-container">
        <div class="wave"></div>
        <div class="wave"></div>
    </div>
    <div style="position: relative; z-index: 1;">
        <h1 style="font-size: 4em; margin-bottom: 10px; text-shadow: 0 0 10px rgba(0, 255, 255, 0.7);">MyStIc-mY</h1>
        <h2 style="font-size: 2em; margin-bottom: 20px; color: #64ffda;">Amit Kumar</h2>
        <p class="typing-text" style="font-size: 1.2em;">Student | Passionate About Cybersecurity & Digital Innovation | Lifelong Learner</p>
    </div>
</div>
