```md
# Orano Project (STILL IN IDEATION PHASE)

**Goal**: A library to benchmark various Large Language Models (LLMs) by:
1. Receiving a prompt from the user.
2. Converting that prompt into step-by-step actions.
3. Interacting with a computer environment (e.g., identifying screen elements, automating tasks).

This project is in its **early stages**, with a vision to evolve into a robust suite of modules for text-driven automation.

---

## Key Modules

1. **Vision**  
   - Captures screenshots and detects objects (e.g., buttons, windows, text fields).
   - Provides metadata about screen elements.

2. **Mind**  
   - Manages prompt handling and interaction with one or more LLMs.
   - Breaks user requests into smaller, sequenced commands.

3. **OranoBot**  
   - Orchestrates the workflow:  
     - Accepts user prompts.  
     - Calls **Mind** to generate actions.  
     - Uses **Vision** to provide environment context (screenshots).  
     - Executes each step on the computer.  

4. **UI** (Optional)  
   - Helper module for user-interface operations, hooking into the OS or external libraries for automation.

---

## Project Status

- **Just Started**: The code structure is set up, but actual implementations are minimal or placeholders.
- **MLOps**: Will be integrated later for continuous model training/deployment, if needed.
- **Docker & AWS**: Planned, but not implemented yet.

---

## Devlog

- We maintain a **development log** in the [`devlog/`](./devlog/) folder.  
  - Each date has its own `.md` file (e.g., `devlog_2024_12_30.md`).  
  - The latest development notes and images are there.  
- We may occasionally highlight the most recent devlog entries here in the main README.
- You can also follow the project on [`medium`](https://medium.com/@henrique382) 

---

## Directory Structure

```
my_orano_project/
├── .gitignore
├── LICENSE
├── README.md
├── devlog/
│   └── imgs/
├── docs/
│   └── architecture.md
├── requirements.txt
├── src/
│   └── orano/
│       ├── __init__.py
│       ├── mind.py
│       ├── vision.py
│       ├── bot.py
│       └── ui.py
└── tests/
    ├── __init__.py
    ├── test_mind.py
    ├── test_vision.py
    ├── test_bot.py
    └── test_ui.py
```

**Notes**:
- `src/orano/` houses your main code modules.
- `tests/` contains unit tests for each module.
- `devlog/` stores the development journal and images.

---

## Getting Started

1. **Clone the Repo**
   ```bash
   git clone git@github.com:Gabriel382/orano.git
   cd orano
   ```

2. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```
   *(If you prefer Poetry or Conda, adjust accordingly.)*

3. **Run Basic Tests**
   ```bash
   pytest tests
   ```
   *(Or your test runner of choice.)*

4. **Explore the Devlog**
   - Check out [`devlog/`](./devlog/) for detailed progress notes and any relevant screenshots or diagrams.

---

## Contributing

- Check out our [LICENSE](./LICENSE) to see how this project is distributed.
- Feel free to open issues or pull requests if you have ideas or bug fixes.
- As we grow, we’ll add a `CONTRIBUTING.md` for guidelines and best practices.

---

## License

This project is licensed under the [MIT License](./LICENSE). Please see the license file for full details.

---

**Happy Building**  
Stay tuned for updates, and check our devlog for day-to-day progress!
```