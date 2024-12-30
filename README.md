<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a id="readme-top"></a>

<!-- PROJECT SHIELDS -->
<!--
  Reference style links for readability.
  Update each [bracketed URL] with your own repo/username, if you'd like to keep these badges.
-->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

<br />
<div align="center">
  <h1>Orano (Ontology-driven Reasoning with AI for Natural Operations) Project <br> STILL IN IDEATION PHASE</h1>
  <p>A library to benchmark various Large Language Models (LLMs) by receiving a prompt from the user, converting it into step-by-step actions, and interacting with a computer environment.</p>
  <a href="https://github.com/Gabriel382/orano"><strong>Explore the Docs »</strong></a>
  <br />
  <br />
  <a href="https://github.com/Gabriel382/orano/issues/new?assignees=&labels=bug&template=bug_report.md&title=">Report Bug</a>
  ·
  <a href="https://github.com/Gabriel382/orano/issues/new?assignees=&labels=enhancement&template=feature_request.md&title=">Request Feature</a>
</div>

---

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#key-modules">Key Modules</a></li>
    <li><a href="#project-status">Project Status</a></li>
    <li><a href="#devlog">Devlog</a></li>
    <li><a href="#directory-structure">Directory Structure</a></li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#clone-the-repo">Clone the Repo</a></li>
        <li><a href="#install-dependencies">Install Dependencies</a></li>
        <li><a href="#run-basic-tests">Run Basic Tests</a></li>
      </ul>
    </li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>

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

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

## Project Status

- **Just Started**: The code structure is set up, but actual implementations are minimal or placeholders.  
- **MLOps**: Will be integrated later for continuous model training/deployment, if needed.  
- **Docker & AWS**: Planned, but not implemented yet.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

## Devlog

- We maintain a **development log** in the [`devlog/`](./devlog/) folder.  
  - Each date has its own `.md` file (e.g., `devlog_2024_12_30.md`).  
  - The latest development notes and images are there.  
- We may occasionally highlight the most recent devlog entries here in the main README.  
- You can also follow the project on [Medium](https://medium.com/@henrique382).

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

## Directory Structure

```
orano/
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

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

## Getting Started

### Clone the Repo
```bash
git clone https://github.com/Gabriel382/orano.git
cd orano
```

### Install Dependencies
```bash
pip install -r requirements.txt
```
*(If you prefer Poetry or Conda, adjust accordingly.)*

### Run Basic Tests
```bash
pytest tests
```
*(Or your test runner of choice.)*

Check out the [`devlog/`](./devlog/) for detailed progress notes and any relevant screenshots or diagrams.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

## Contributing

- Check out our [LICENSE](./LICENSE) to see how this project is distributed.  
- Feel free to open issues or pull requests if you have ideas or bug fixes.  
- As we grow, we’ll add a `CONTRIBUTING.md` for guidelines and best practices.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

## License

This project is licensed under the [MIT License](./LICENSE). Please see the license file for full details.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

## Contact

**Gabriel Henrique Alencar Medeiros**  
- [LinkedIn Profile](https://www.linkedin.com/in/gabriel-henrique-am/?locale=en_US)  
- [GitHub Repository](https://github.com/Gabriel382/orano)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

**Happy Building!**  
Stay tuned for updates, and check our devlog for day-to-day progress.

<!-- MARKDOWN LINKS & IMAGES -->
<!-- Replace the bracketed text with your repo details or remove if you don't want badges -->
[contributors-shield]: https://img.shields.io/github/contributors/Gabriel382/orano.svg?style=for-the-badge
[contributors-url]: https://github.com/Gabriel382/orano/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/Gabriel382/orano.svg?style=for-the-badge
[forks-url]: https://github.com/Gabriel382/orano/network/members
[stars-shield]: https://img.shields.io/github/stars/Gabriel382/orano.svg?style=for-the-badge
[stars-url]: https://github.com/Gabriel382/orano/stargazers
[issues-shield]: https://img.shields.io/github/issues/Gabriel382/orano.svg?style=for-the-badge
[issues-url]: https://github.com/Gabriel382/orano/issues
[license-shield]: https://img.shields.io/github/license/Gabriel382/orano.svg?style=for-the-badge
[license-url]: https://github.com/Gabriel382/orano/blob/main/LICENSE
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/gabriel-henrique-am/?locale=en_US
