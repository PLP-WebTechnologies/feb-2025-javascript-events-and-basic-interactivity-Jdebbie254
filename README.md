# 🎯 JavaScript Event Handling & Interactive Elements Assignment

Welcome to the **ultimate JavaScript playground**! 🎉 This assignment is where we turn boring web pages into dynamic, responsive, *alive* experiences. Get ready to master **event handling**, build **interactive components**, and validate forms like a pro! 💪

## 📁 Assignment Structure

```
📂 js-event-assignment/
├── index.html         # Your playground – where it all comes together
├── style.css          # Keep it cute (optional but encouraged)
└── script.js          # The JavaScript wizardry happens here
```

---

## 🧪 What to Build

Here’s what your interactive bundle of joy should include:

### 1. Event Handling 🎈  
- Button click ✅  
- Hover effects ✅  
- Keypress detection ✅  
- Bonus: A secret action for a *double-click* or *long press* 🤫

### 2. Interactive Elements 🎮  
- A button that changes text or color  
- An image gallery or slideshow  
- Tabs or accordion-style content  
- Bonus: Add some animation using JS or CSS ✨

### 3. Form Validation 📋✅  
- Required field checks  
- Email format validation  
- Password rules (e.g., min 8 characters)  
- Bonus: Real-time feedback while typing

---

## 🧙‍♂️ Pro Tips

- Keep your code clean and commented – your future self will thank you!
- Think about **user experience** – what makes your site more *fun* to use?
- Don’t be afraid to **Google and experiment** – that’s how real developers roll!

- ## 🎉 Now Go Make It Fun!

Remember – this isn't just code. It's your **first step toward creating magical user experiences**. So play around, break stuff (then fix it), and most of all, have FUN! 😄

Happy Coding! 💻✨  

📂 js-event-assignment/
├── index.html         # Main HTML file with all elements
├── style.css          # Styles for the interactive components
└── script.js          # JavaScript for event handling and interactivity

.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive JavaScript Playground</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>JavaScript Interactive Playground</h1>
        <p>Explore event handling and interactive elements</p>
    </header>

    <main>
        <!-- Event Handling Section -->
        <section id="event-section">
            <h2>Event Handling</h2>
            
            <div class="event-box">
                <h3>Button Click</h3>
                <button id="click-btn" class="event-btn">Click Me!</button>
                <p id="click-output">Waiting for your click...</p>
            </div>
            
            <div class="event-box">
                <h3>Hover Effects</h3>
                <div id="hover-box" class="interactive-box">Hover over me!</div>
            </div>
            
            <div class="event-box">
                <h3>Keypress Detection</h3>
                <input type="text" id="keypress-input" placeholder="Type something...">
                <p id="keypress-output">You pressed: </p>
            </div>
            
            <div class="event-box">
                <h3>Secret Action (Double Click)</h3>
                <div id="secret-box" class="interactive-box">Double click me for a surprise!</div>
            </div>
        </section>

        <!-- Interactive Elements Section -->
        <section id="interactive-section">
            <h2>Interactive Elements</h2>
            
            <div class="interactive-box">
                <h3>Color Changer</h3>
                <button id="color-changer" class="event-btn">Change Color</button>
                <div id="color-display"></div>
            </div>
            
            <div class="interactive-box">
                <h3>Image Gallery</h3>
                <div class="gallery">
                    <img id="gallery-image" src="https://picsum.photos/id/10/400/300" alt="Gallery image">
                    <div class="gallery-controls">
                        <button id="prev-btn">← Previous</button>
                        <button id="next-btn">Next →</button>
                    </div>
                </div>
            </div>
            
            <div class="interactive-box">
                <h3>Accordion</h3>
                <div class="accordion">
                    <div class="accordion-item">
                        <button class="accordion-btn">Section 1</button>
                        <div class="accordion-content">
                            <p>Content for section 1 goes here.</p>
                        </div>
                    </div>
                    <div class="accordion-item">
                        <button class="accordion-btn">Section 2</button>
                        <div class="accordion-content">
                            <p>Content for section 2 goes here.</p>
                        </div>
                    </div>
                    <div class="accordion-item">
                        <button class="accordion-btn">Section 3</button>
                        <div class="accordion-content">
                            <p>Content for section 3 goes here.</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Form Validation Section -->
        <section id="form-section">
            <h2>Form Validation</h2>
            <form id="demo-form">
                <div class="form-group">
                    <label for="name">Name*:</label>
                    <input type="text" id="name" name="name" required>
                    <div class="error-message" id="name-error"></div>
                </div>
                
                <div class="form-group">
                    <label for="email">Email*:</label>
                    <input type="email" id="email" name="email" required>
                    <div class="error-message" id="email-error"></div>
                </div>
                
                <div class="form-group">
                    <label for="password">Password* (min 8 chars):</label>
                    <input type="password" id="password" name="password" required minlength="8">
                    <div class="error-message" id="password-error"></div>
                    <div class="password-strength">
                        <span class="strength-meter"></span>
                        <span class="strength-text"></span>
                    </div>
                </div>
                
                <button type="submit" class="submit-btn">Submit</button>
                <div id="form-success" class="success-message"></div>
            </form>
        </section>
    </main>

    <footer>
        <p>JavaScript Interactive Playground &copy; 2023</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>

.css
/* Base Styles */
body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    line-height: 1.6;
    margin: 0;
    padding: 20px;
    background-color: #f5f5f5;
    color: #333;
}

header, main, footer {
    max-width: 1000px;
    margin: 0 auto;
    padding: 20px;
}

header {
    text-align: center;
    margin-bottom: 30px;
}

h1, h2, h3 {
    color: #2c3e50;
}

section {
    background-color: white;
    border-radius: 8px;
    padding: 20px;
    margin-bottom: 30px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
}

/* Event Handling Styles */
.event-box, .interactive-box {
    margin-bottom: 20px;
    padding: 15px;
    border: 1px solid #ddd;
    border-radius: 5px;
}

.event-btn {
    background-color: #3498db;
    color: white;
    border: none;
    padding: 10px 15px;
    border-radius: 4px;
    cursor: pointer;
    font-size: 16px;
    transition: background-color 0.3s;
}

.event-btn:hover {
    background-color: #2980b9;
}

.interactive-box {
    padding: 20px;
    margin: 10px 0;
    background-color: #f9f9f9;
    border-radius: 5px;
    transition: all 0.3s;
}

#hover-box {
    height: 100px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-weight: bold;
}

#secret-box {
    height: 80px;
    display: flex;
    align-items: center;
    justify-content: center;
    cursor: pointer;
}

#color-display {
    height: 100px;
    width: 100%;
    margin-top: 10px;
    border-radius: 5px;
    background-color: #e74c3c;
    transition: background-color 0.5s;
}

/* Gallery Styles */
.gallery {
    text-align: center;
}

.gallery img {
    max-width: 100%;
    height: auto;
    border-radius: 5px;
    margin-bottom: 10px;
}

.gallery-controls {
    display: flex;
    justify-content: center;
    gap: 10px;
}

/* Accordion Styles */
.accordion-item {
    margin-bottom: 5px;
}

.accordion-btn {
    width: 100%;
    text-align: left;
    padding: 10px 15px;
    background-color: #ecf0f1;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    font-size: 16px;
    transition: background-color 0.3s;
}

.accordion-btn:hover {
    background-color: #bdc3c7;
}

.accordion-content {
    padding: 0 15px;
    max-height: 0;
    overflow: hidden;
    transition: max-height 0.3s ease-out;
    background-color: white;
    border-radius: 0 0 4px 4px;
}

.accordion-content.active {
    padding: 15px;
    max-height: 500px;
}

/* Form Styles */
.form-group {
    margin-bottom: 15px;
}

.form-group label {
    display: block;
    margin-bottom: 5px;
    font-weight: bold;
}

.form-group input {
    width: 100%;
    padding: 10px;
    border: 1px solid #ddd;
    border-radius: 4px;
    font-size: 16px;
}

.error-message {
    color: #e74c3c;
    font-size: 14px;
    margin-top: 5px;
    height: 20px;
}

.success-message {
    color: #2ecc71;
    font-size: 16px;
    margin-top: 15px;
    text-align: center;
    font-weight: bold;
}

.password-strength {
    margin-top: 10px;
}

.strength-meter {
    display: inline-block;
    height: 5px;
    width: 0;
    background-color: #e74c3c;
    transition: width 0.3s, background-color 0.3s;
}

.strength-text {
    margin-left: 10px;
    font-size: 14px;
    color: #7f8c8d;
}

.submit-btn {
    background-color: #2ecc71;
    color: white;
    border: none;
    padding: 12px 20px;
    border-radius: 4px;
    cursor: pointer;
    font-size: 16px;
    width: 100%;
    transition: background-color 0.3s;
}

.submit-btn:hover {
    background-color: #27ae60;
}

/* Animation */
@keyframes shake {
    0%, 100% { transform: translateX(0); }
    20%, 60% { transform: translateX(-5px); }
    40%, 80% { transform: translateX(5px); }
}

.shake {
    animation: shake 0.5s;
}

.js
document.addEventListener('DOMContentLoaded', function() {
    // ========== Event Handling ==========
    
    // Button Click Event
    const clickBtn = document.getElementById('click-btn');
    const clickOutput = document.getElementById('click-output');
    
    clickBtn.addEventListener('click', function() {
        clickOutput.textContent = "You clicked the button! Great job! 🎉";
        clickOutput.style.color = "#2ecc71";
    });
    
    // Hover Effects
    const hoverBox = document.getElementById('hover-box');
    
    hoverBox.addEventListener('mouseenter', function() {
        this.textContent = "Mouse is over me! 😊";
        this.style.backgroundColor = "#3498db";
        this.style.color = "white";
    });
    
    hoverBox.addEventListener('mouseleave', function() {
        this.textContent = "Hover over me!";
        this.style.backgroundColor = "#f9f9f9";
        this.style.color = "#333";
    });
    
    // Keypress Detection
    const keypressInput = document.getElementById('keypress-input');
    const keypressOutput = document.getElementById('keypress-output');
    
    keypressInput.addEventListener('keyup', function(e) {
        keypressOutput.textContent = `You pressed: ${e.key} (Key code: ${e.keyCode})`;
    });
    
    // Secret Action (Double Click)
    const secretBox = document.getElementById('secret-box');
    
    secretBox.addEventListener('dblclick', function() {
        this.textContent = "🎉 Surprise! You found the secret! 🎉";
        this.style.backgroundColor = "#9b59b6";
        this.style.color = "white";
        
        // Reset after 2 seconds
        setTimeout(() => {
            this.textContent = "Double click me for a surprise!";
            this.style.backgroundColor = "#f9f9f9";
            this.style.color = "#333";
        }, 2000);
    });
    
    // ========== Interactive Elements ==========
    
    // Color Changer
    const colorChanger = document.getElementById('color-changer');
    const colorDisplay = document.getElementById('color-display');
    
    colorChanger.addEventListener('click', function() {
        const colors = ['#e74c3c', '#3498db', '#2ecc71', '#f1c40f', '#9b59b6', '#1abc9c'];
        const randomColor = colors[Math.floor(Math.random() * colors.length)];
        colorDisplay.style.backgroundColor = randomColor;
    });
    
    // Image Gallery
    const galleryImage = document.getElementById('gallery-image');
    const prevBtn = document.getElementById('prev-btn');
    const nextBtn = document.getElementById('next-btn');
    
    const images = [
        { id: 10, alt: "Forest" },
        { id: 11, alt: "Desert" },
        { id: 12, alt: "Ocean" },
        { id: 13, alt: "Mountain" },
        { id: 14, alt: "Field" }
    ];
    
    let currentImageIndex = 0;
    
    function updateGalleryImage() {
        const img = images[currentImageIndex];
        galleryImage.src = `https://picsum.photos/id/${img.id}/400/300`;
        galleryImage.alt = img.alt;
    }
    
    prevBtn.addEventListener('click', function() {
        currentImageIndex = (currentImageIndex - 1 + images.length) % images.length;
        updateGalleryImage();
    });
    
    nextBtn.addEventListener('click', function() {
        currentImageIndex = (currentImageIndex + 1) % images.length;
        updateGalleryImage();
    });
    
    // Accordion
    const accordionBtns = document.querySelectorAll('.accordion-btn');
    
    accordionBtns.forEach(btn => {
        btn.addEventListener('click', function() {
            this.classList.toggle('active');
            const content = this.nextElementSibling;
            
            if (content.classList.contains('active')) {
                content.classList.remove('active');
            } else {
                // Close all other accordion items
                document.querySelectorAll('.accordion-content').forEach(item => {
                    item.classList.remove('active');
                });
                document.querySelectorAll('.accordion-btn').forEach(item => {
                    item.classList.remove('active');
                });
                
                // Open current one
                content.classList.add('active');
                this.classList.add('active');
            }
        });
    });
    
    // ========== Form Validation ==========
    const demoForm = document.getElementById('demo-form');
    const nameInput = document.getElementById('name');
    const emailInput = document.getElementById('email');
    const passwordInput = document.getElementById('password');
    const nameError = document.getElementById('name-error');
    const emailError = document.getElementById('email-error');
    const passwordError = document.getElementById('password-error');
    const formSuccess = document.getElementById('form-success');
    const strengthMeter = document.querySelector('.strength-meter');
    const strengthText = document.querySelector('.strength-text');
    
    // Real-time validation
    nameInput.addEventListener('input', validateName);
    emailInput.addEventListener('input', validateEmail);
    passwordInput.addEventListener('input', validatePassword);
    
    function validateName() {
        if (nameInput.value.trim() === '') {
            nameError.textContent = 'Name is required';
            nameInput.classList.add('invalid');
            return false;
        } else if (nameInput.value.trim().length < 2) {
            nameError.textContent = 'Name must be at least 2 characters';
            nameInput.classList.add('invalid');
            return false;
        } else {
            nameError.textContent = '';
            nameInput.classList.remove('invalid');
            return true;
        }
    }
    
    function validateEmail() {
        const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
        
        if (emailInput.value.trim() === '') {
            emailError.textContent = 'Email is required';
            emailInput.classList.add('invalid');
            return false;
        } else if (!emailRegex.test(emailInput.value)) {
            emailError.textContent = 'Please enter a valid email';
            emailInput.classList.add('invalid');
            return false;
        } else {
            emailError.textContent = '';
            emailInput.classList.remove('invalid');
            return true;
        }
    }
    
    function validatePassword() {
        const password = passwordInput.value;
        
        if (password === '') {
            passwordError.textContent = 'Password is required';
            strengthMeter.style.width = '0';
            strengthText.textContent = '';
            passwordInput.classList.add('invalid');
            return false;
        } else if (password.length < 8) {
            passwordError.textContent = 'Password must be at least 8 characters';
            strengthMeter.style.width = '25%';
            strengthMeter.style.backgroundColor = '#e74c3c';
            strengthText.textContent = 'Weak';
            strengthText.style.color = '#e74c3c';
            passwordInput.classList.add('invalid');
            return false;
        } else {
            passwordError.textContent = '';
            passwordInput.classList.remove('invalid');
            
            // Calculate password strength
            let strength = 0;
            if (password.length >= 8) strength += 1;
            if (/[A-Z]/.test(password)) strength += 1;
            if (/[0-9]/.test(password)) strength += 1;
            if (/[^A-Za-z0-9]/.test(password)) strength += 1;
            
            // Update strength meter
            const width = (strength / 4) * 100;
            strengthMeter.style.width = `${width}%`;
            
            if (strength <= 1) {
                strengthMeter.style.backgroundColor = '#e74c3c';
                strengthText.textContent = 'Weak';
                strengthText.style.color = '#e74c3c';
            } else if (strength <= 3) {
                strengthMeter.style.backgroundColor = '#f39c12';
                strengthText.textContent = 'Medium';
                strengthText.style.color = '#f39c12';
            } else {
                strengthMeter.style.backgroundColor = '#2ecc71';
                strengthText.textContent = 'Strong';
                strengthText.style.color = '#2ecc71';
            }
            
            return true;
        }
    }
    
    // Form submission
    demoForm.addEventListener('submit', function(e) {
        e.preventDefault();
        
        const isNameValid = validateName();
        const isEmailValid = validateEmail();
        const isPasswordValid = validatePassword();
        
        if (isNameValid && isEmailValid && isPasswordValid) {
            formSuccess.textContent = 'Form submitted successfully! 🎉';
            
            // Reset form after 2 seconds
            setTimeout(() => {
                demoForm.reset();
                formSuccess.textContent = '';
                strengthMeter.style.width = '0';
                strengthText.textContent = '';
            }, 2000);
        } else {
            // Add shake animation to invalid fields
            if (!isNameValid) nameInput.classList.add('shake');
            if (!isEmailValid) emailInput.classList.add('shake');
            if (!isPasswordValid) passwordInput.classList.add('shake');
            
            // Remove shake class after animation completes
            setTimeout(() => {
                nameInput.classList.remove('shake');
                emailInput.classList.remove('shake');
                passwordInput.classList.remove('shake');
            }, 500);
        }
    });
});
---


