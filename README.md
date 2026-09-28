# WayFinder

WayFinder is a beginner-friendly web app designed to help learners understand their current position in a learning path and identify what they should learn next.

Instead of simply providing a long list of topics, WayFinder uses the user's existing skills to determine their current stage and provide a clearer direction for their next steps.

The project is currently focused on the **AI Engineer learning path**.

## Features

- **Learning Path Selection:** Choose a learning path based on your career goal.
- **Skill Tracking:** Select skills you already know and skills you are still unsure about. Unselected skills are treated as not learned yet.
- **Learning Stage Detection:** Automatically identifies your current learning stage based on your selected skills.
- **Progress Overview:** Displays your learning goal, current stage, completed skills, and remaining skills.
- **Next-Step Guidance:** Identifies the next skill you should focus on.
- **Learning Resources:** Provides relevant learning resources for skills in the roadmap.
- **AI Learning Assistant:** Ask questions about your learning progress and current topics with context from your WayFinder profile.
- **Error Handling:** Handles invalid inputs and API-related errors with fallback responses.

## How It Works

The basic flow of WayFinder is:

1. The user selects a learning goal.
2. The user selects the skills they already know or are unsure about.
3. WayFinder compares the selected skills with the learning roadmap.
4. WayFinder determines the user's current learning stage.
5. The application identifies the next skill to focus on.
6. The user can explore relevant learning resources and the full roadmap.
7. The AI Learning Assistant can answer questions related to the user's learning progress.

The AI assistant receives relevant learning context from WayFinder, including the user's learned skills, unsure skills, current stage, and next step. This allows its responses to be more relevant to the user's current learning position.

## Technologies

- Python
- Flask
- HTML
- CSS
- JavaScript
- JSON
- Groq API
- Git
- GitHub

## Project Structure

```text
way-finder/
├── data/
│   └── learning_map.json
├── static/
│   └── style.css
├── templates/
│   ├── index.html
│   └── result.html
├── .env.example
├── app.py
└── requirements.txt
```

## Setup & Installation

Make sure you have Python and Git installed on your machine.

### 1. Clone the repository
```bash
git clone https://github.com/yelzz-hub/way-finder.git
cd way-finder
```

### 2. Create and activate a virtual environment

*   **Windows:**
    ```bash
    python -m venv venv
    venv\Scripts\activate
    ```
*   **macOS / Linux:**
    ```bash
    python3 -m venv venv
    source venv/bin/activate
    ```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Configure environment variables

Create a `.env` file in the root directory based on `.env.example` and add the required environment variables:

```text
GROQ_API_KEY=your_api_key_here
FLASK_SECRET_KEY=your_secret_key_here
```
>  **Important:** Do not share your real API keys publicly or commit your `.env` file to GitHub.

### 5. Run the application
```bash
flask --app app run
```

Once the application is running, open your browser and navigate to:  
**`http://127.0.0.1:5000`**

## AI Usage

AI tools were used during the development of WayFinder as learning and development assistance.

AI was used for:

- **Brainstorming:** Project ideas and core features.
- **Learning:** Understanding programming concepts and framework behavior.
- **Debugging:** Syntax, runtime, and logic errors.
- **Implementation:** Discussing implementation approaches.
- **Testing:** Exploring edge cases and different user scenarios.
- **Documentation & UX:** Improving documentation explanations and user experience.
- **AI Assistant:** Testing and refining the conversational behavior of the AI Learning Assistant.

The project was developed and tested by the participant, with AI used as a learning and development assistant. AI was used for learning and development assistance rather than as a replacement for understanding the codebase.


## External Resources & Credits

WayFinder uses the following technologies and external resources:

- **Flask** — Python web framework used to build the application.
- **Groq API** — AI API used by the Learning Assistant.
- **Marked** — Markdown parser used to render AI responses.
- **DOMPurify** — Used to sanitize rendered AI responses.
- **Learning Resources** — External educational resources referenced in the learning roadmap.

All external resources are credited where applicable.


## Development Process

The development process was carried out through the following stages:

- **Project Initialization:** Creating the initial Flask application and setting up the development environment.
- **Roadmap Design:** Designing and structuring the learning roadmap data.
- **Core Logic:** Building the skill-matching system and implementing learning stage detection.
- **Progress Tracking:** Calculating learning progress based on the user's selected skills.
- **Frontend Development:** Building the learning roadmap and progress user interface.
- **AI Integration:** Integrating the AI Learning Assistant with the user's current learning context.
- **Error Handling:** Adding validation and fallback responses for invalid input and API errors.
- **Testing:** Testing different combinations of learned and unsure skills, including edge cases.
- **Refactoring & UI Polish:** Improving the code structure and refining the application's user interface.

The project's GitHub repository contains the development history through multiple meaningful commits.

## Author

- **Developed by:** Yelizaveta S
