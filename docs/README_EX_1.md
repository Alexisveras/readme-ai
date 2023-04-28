
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>
README-AI
</h1>
<h3 align="center">📍 Unlock the Power of Automation with README-AI</h3>
<h3 align="center">🚀 Developed with the software and tools below.</h3>
<p align="center">

<img src="https://img.shields.io/badge/OpenAI-412991.svg?style=for-the-badge&logo=OpenAI&logoColor=white" alt="" />
<img src="https://img.shields.io/badge/pandas-150458.svg?style=for-the-badge&logo=pandas&logoColor=white" alt="dacite" />
<img src="https://img.shields.io/badge/Markdown-000000.svg?style=for-the-badge&logo=Markdown&logoColor=white" alt="sample" />
<img src="https://img.shields.io/badge/JSON-000000.svg?style=for-the-badge&logo=JSON&logoColor=white" alt="flake8" />

<img src="https://img.shields.io/badge/Python-3776AB.svg?style=for-the-badge&logo=Python&logoColor=white" alt="idx" />
<img src="https://img.shields.io/badge/Pytest-0A9EDC.svg?style=for-the-badge&logo=Pytest&logoColor=white" alt="pandas" />
<img src="https://img.shields.io/badge/spaCy-09A3D5.svg?style=for-the-badge&logo=spaCy&logoColor=white" alt="colorlog" />
<img src="https://img.shields.io/badge/GNU%20Bash-4EAA25.svg?style=for-the-badge&logo=GNU-Bash&logoColor=white" alt="json" />
<img src="https://img.shields.io/badge/precommit-FAB040.svg?style=for-the-badge&logo=pre-commit&logoColor=black" alt="spacy" />
</p>

</div>

---
## 📚 Table of Contents
- [📚 Table of Contents](#-table-of-contents)
- [📍Overview](#overview)
- [🔮 Feautres](#-feautres)
- [⚙️ Project Structure](#️-project-structure)
- [💻 Modules](#-modules)
- [🚀 Getting Started](#-getting-started)
  - [✅ Prerequisites](#-prerequisites)
  - [💻 Installation](#-installation)
  - [🤖 Using README-AI](#-using-readme-ai)
  - [🧪 Running Tests](#-running-tests)
- [🛠 Future Development](#-future-development)
- [🤝 Contributing](#-contributing)
- [🪪 License](#-license)
- [🙏 Acknowledgments](#-acknowledgments)

---

## 📍Overview

README-AI is a machine learning project that generates template-based README files for GitHub repositories. It automates the process of creating a README and reduces the time needed to write a README.

## 🔮 Feautres

> `[📌  INSERT-PROJECT-FEATURES]`

---

<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-github-open.svg" width="80" />

## ⚙️ Project Structure

```bash
.
├── CONTRIBUTING.md
├── LICENSE
├── Makefile
├── README.md
├── conf
│   ├── badges.json
│   ├── conf.toml
│   ├── file_extensions.toml
│   ├── file_names.toml
│   ├── ignore_files.toml
│   ├── setup_guide.toml
│   └── templates
│       └── general.toml
├── docs
│   ├── README_EX_1.md
│   ├── README_EX_2.md
│   ├── README_EX_3.md
│   ├── README_EX_GO.md
│   ├── README_EX_JS.md
│   ├── README_EX_RUST.md
│   └── imgs
│       ├── docs.png
│       ├── header.png
│       ├── misc.png
│       ├── setup.png
│       ├── toc.png
│       └── tree.png
├── requirements.txt
├── scripts
│   ├── clean.sh
│   ├── run.sh
│   └── test.sh
├── setup
│   ├── environment.yaml
│   └── setup.sh
├── setup.py
├── src
│   ├── __init__.py
│   ├── builder.py
│   ├── conf.py
│   ├── file_factory.py
│   ├── logger.py
│   ├── main.py
│   ├── model.py
│   ├── preprocess.py
│   └── preprocess_helper.py
└── tests
    ├── conftest.py
    ├── test_builder.py
    ├── test_conf.py
    ├── test_file_factory.py
    ├── test_logger.py
    ├── test_main.py
    ├── test_model.py
    ├── test_preprocess.py
    └── test_preprocess_helper.py

9 directories, 48 files
```
---

<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-src-open.svg" width="80" />

## 💻 Modules
<details closed><summary>Scripts</summary>

| File     | Summary                                                                                                                                                                                                                    | Module           |
|:---------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------------|
| run.sh   | This code is a Bash script that activates a Conda environment and runs a Python script. It also allows for the exporting of environment variables.                                                                         | scripts/run.sh   |
| clean.sh | This code is a Bash script that deletes files and directories related to Python, Jupyter notebooks, pytest, benchmarks, logs, and a CSV file.                                                                              | scripts/clean.sh |
| test.sh  | This code is a Bash script that activates a conda environment, sets the directories to include and exclude in a coverage report, generates the coverage report and saves it to a file, and then removes files and folders. | scripts/test.sh  |

</details>

<details closed><summary>Src</summary>

| File                 | Summary                                                                                                                                                                                                                                                                          | Module                   |
|:---------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-------------------------|
| preprocess.py        | This code preprocesses a codebase to extract the README. md file and other code files. It clones the codebase from a remote repository or uses a local directory, then parses the files to extract the contents.                                                                 | src/preprocess.py        |
| conf.py              | This code defines configuration constants for an application, including OpenAI API details, GitHub repository details, Markdown template strings, and project paths.                                                                                                             | src/conf.py              |
| preprocess_helper.py | This code provides helper functions for dependency parsing for README-AI. It includes functions for parsing Conda environment files, Pipfiles, pyproject. toml, requirements files, Cargo. toml, Cargo. lock, package. json, yarn. lock, Go module files, and Go sum files.      | src/preprocess_helper.py |
| logger.py            | This code is a custom logger module using loguru for README-AI. It provides functions for logging messages at different levels, such as info, debug, warning, error, critical, trace, success, and exception.                                                                    | src/logger.py            |
| file_factory.py      | This module provides a FileHandler class that can read and write files in markdown, toml, and json formats. It provides methods to read and write files in these formats, as well as a get_action method to retrieve the appropriate read or write action for a given file type. | src/file_factory.py      |
| model.py             | This code is an OpenAI API handler for generating text for the README. md file. It uses the OpenAI GPT-3 API to generate summary descriptions for code files, and the SpaCy library to summarize text.                                                                           | src/model.py             |
| builder.py           | This code builds a README. md file from a template and data, such as a pandas DataFrame, a configuration object, and a list of dependencies.                                                                                                                                     | src/builder.py           |
| main.py              | README-AI is a tool that uses OpenAI's API to generate a README. md file for a given repository. It collects information from the repository, such as project dependencies and codebase summaries, and uses this data to create a comprehensive README. md file.                 | src/main.py              |

</details>
<hr />

## 🚀 Getting Started

### ✅ Prerequisites

Before you begin, ensure that you have the following prerequisites installed:
> `[📌  INSERT-PROJECT-PREREQUISITES]`

### 💻 Installation

1. Clone the README-AI repository:
```sh
git clone https://github.com/eli64s/README-AI
```

2. Change to the project directory:
```sh
cd README-AI
```

3. Install the dependencies:
```sh
pip install -r requirements.txt
```

### 🤖 Using README-AI

```sh
python main.py
```

### 🧪 Running Tests
```sh
#run tests
```

<hr />

## 🛠 Future Development
- [X] [📌  COMPLETED-TASK]
- [ ] [📌  INSERT-TASK]
- [ ] [📌  INSERT-TASK]


---

## 🤝 Contributing
Contributions are always welcome! Please follow these steps:
1. Fork the project repository. This creates a copy of the project on your account that you can modify without affecting the original project.
2. Clone the forked repository to your local machine using a Git client like Git or GitHub Desktop.
3. Create a new branch with a descriptive name (e.g., `new-feature-branch` or `bugfix-issue-123`).
```sh
git checkout -b new-feature-branch
```
4. Make changes to the project's codebase.
5. Commit your changes to your local branch with a clear commit message that explains the changes you've made.
```sh
git commit -m 'Implemented new feature.'
```
6. Push your changes to your forked repository on GitHub using the following command
```sh
git push origin new-feature-branch
```
7. Create a pull request to the original repository.
Open a new pull request to the original project repository. In the pull request, describe the changes you've made and why they're necessary.
The project maintainers will review your changes and provide feedback or merge them into the main branch.

---

## 🪪 License

This project is licensed under the `[📌  INSERT-LICENSE-TYPE]` License. See the [LICENSE](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/adding-a-license-to-a-repository) file for additional info.

---

## 🙏 Acknowledgments

[📌  INSERT-DESCRIPTION]


---
