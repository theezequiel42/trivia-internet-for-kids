# Internet Safety Quiz Game - Interactive Learning for Digital Citizenship

This project is an engaging web-based quiz game designed to teach internet safety and responsible online behavior through interactive questions and immediate feedback. The game combines educational content with gamification elements to make learning about digital citizenship both fun and effective.

The quiz game features a user-friendly interface with three distinct screens (Welcome, Quiz, and Results) and incorporates visual feedback through emojis and color-coded responses. Built using modern web technologies including Tailwind CSS for styling and responsive design, the game provides an accessible learning experience that works across different devices and screen sizes.

## Repository Structure
```
.
└── index.html              # Single-page application containing HTML, CSS, and JavaScript for the quiz game
```

## Usage Instructions
### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, or Edge)
- Internet connection for loading CDN resources:
  - Tailwind CSS
  - Font Awesome
  - Inter font family
  - Tone.js

### Installation
1. Clone the repository or download the index.html file
2. No build process required - simply open index.html in a web browser

For local development:
```bash
# Using Python's built-in HTTP server
python -m http.server 8000

# Using Node.js's http-server (requires npm install -g http-server)
http-server
```

### Quick Start
1. Open index.html in a web browser
2. Click "Começar Jogo" (Start Game) to begin
3. Read each question carefully and select your answer
4. Receive immediate feedback on your choice
5. Click "Próxima Pergunta" (Next Question) to continue
6. View your final score and performance message at the end

### More Detailed Examples
Example Question Flow:
```javascript
// Sample question interaction
1. Question: "É seguro compartilhar sua senha com colegas?"
   Options: 
   - "Sim, se forem meus amigos."
   - "Não, senhas são como escovas de dente, são pessoais."
   - "Só se for uma senha simples."
   
   Correct Answer: "Não, senhas são como escovas de dente, são pessoais."
   Feedback: "Muito bem! Sua senha é um segredo, não compartilhe com ninguém."
```

### Troubleshooting
Common Issues:
1. Blank/White Screen
   - Check if JavaScript is enabled in your browser
   - Verify internet connection for CDN resources
   - Clear browser cache and reload

2. Style Issues
   - Ensure Tailwind CSS CDN is accessible
   - Check if your browser supports modern CSS features
   - Try hard-refreshing the page (Ctrl+F5 or Cmd+Shift+R)

3. Font Not Loading
   - Verify internet connection
   - Check if Google Fonts is accessible in your region
   - Try using a VPN if Google Fonts is blocked

## Data Flow
The quiz game processes user interactions through a linear question-answer flow, tracking scores and providing immediate feedback.

```ascii
[Welcome Screen] -> [Question Display] -> [User Selection] -> [Feedback] -> [Next Question] -> [Results Screen]
     |                     ^                     |              |              |                    |
     |                     |                     v              v              |                    |
     +---------------------+--------------------[Score Tracking]---------------+--------------------+
```

Component Interactions:
1. Welcome screen initializes game state and waits for user input
2. Quiz screen loads questions from predefined array
3. User selection triggers answer validation
4. Feedback system updates visual and textual responses
5. Score tracking maintains running total
6. Navigation system controls screen transitions
7. Results screen calculates final score and displays performance message