
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>
README AI
</h1>

> <h3 align="center">
>
> `[📌  INSERT-PROJECT-SUMMARY]`
>
> </h3>
> <h3 align="center">🚀 Developed using OpenAI's language model API and the software tools below.</h3>
> <p align="center">
> 
> ![openai](https://img.shields.io/badge/OpenAI-412991.svg?style=for-the-badge&logo=OpenAI&logoColor=white)
> ![pandas](https://img.shields.io/badge/pandas-150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
> ![py](https://img.shields.io/badge/Python-3776AB.svg?style=for-the-badge&logo=Python&logoColor=white)
> ![pytest](https://img.shields.io/badge/Pytest-0A9EDC.svg?style=for-the-badge&logo=Pytest&logoColor=white)
> ![sh](https://img.shields.io/badge/GNU%20Bash-4EAA25.svg?style=for-the-badge&logo=GNU-Bash&logoColor=white)
> ![json](https://img.shields.io/badge/JSON-000000.svg?style=for-the-badge&logo=JSON&logoColor=white)
> ![markdown](https://img.shields.io/badge/Markdown-000000.svg?style=for-the-badge&logo=Markdown&logoColor=white)
> </p>

</div>


---

## 📦 Table of Contents


- [📦 Table of Contents](#-table-of-contents)
- [👋 Introduction](#-introduction)
- [🔮 Feautres](#-feautres)
- [⚙️ Repository Structure](#️-repository-structure)
- [🧩 Modules](#-modules)
- [🏎💨 Getting Started](#-getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Running README AI](#running-readme-ai)
- [🗺 Roadmap](#-roadmap)
- [🤝 Contributing](#-contributing)
- [🪪 License](#-license)
- [📫 Contact](#-contact)
- [🙏 Acknowledgments](#-acknowledgments)

---
## 👋 Introduction

This repository contains a README file generator AI.

## 🔮 Feautres

This project features:

* A README.md file generated automatically by a machine learning model, based on the project's other files
* The ability to generate a README.md file for any GitHub project, using the same machine learning model

---

<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-github-open.svg" width="80" />

## ⚙️ Repository Structure
```bash
.
├── LICENSE
├── Makefile
├── README.md
├── conf
│   ├── badges.json
│   ├── conf.toml
│   └── templates
│       └── base_py.toml
├── docs
│   ├── imgs
│   │   ├── docs.png
│   │   ├── head.png
│   │   ├── misc.png
│   │   ├── tree.png
│   │   └── usage.png
│   ├── raw_data.csv
│   ├── readme_ex1.md
│   └── readme_ex2.md
├── pyproject.toml
├── requirements.txt
├── scripts
│   ├── run_main.sh
│   └── test.sh
├── setup
│   ├── environment.yaml
│   └── setup.sh
├── setup.py
├── src
│   ├── __init__.py
│   ├── builder.py
│   ├── conf.py
│   ├── logger.py
│   ├── main.py
│   ├── model.py
│   ├── processor.py
│   └── utils.py
└── tests
    ├── conftest.py
    ├── test_builder.py
    ├── test_conf.py
    ├── test_logger.py
    ├── test_main.py
    ├── test_model.py
    ├── test_processor.py
    └── test_utils.py

9 directories, 37 files
```
---

<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-src-open.svg" width="80" />

## 🧩 Modules


<details closed><summary>SRC</summary>

| File Name    | Summary                                                                                                                                                                                                                        |
|:-------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| conf.py      | This code defines a configuration constants object, AppConfig, which contains five dataclasses: OpenAI, GitHub, Markdown, Paths, and AppConfig.                                                                                |
| processor.py | This code is a Python script that clones a Git repository and retrieves its contents. It also parses the codebase, gets the file extensions and packages, creates a temporary directory, and creates a conda environment file. |
| logger.py    | This code creates a Logger class which provides methods for logging messages with different levels of severity. It also configures the logger to output messages with colored formatting.                                      |
| model.py     | This code is a Python module that provides functions for summarizing code and generating readme sections. It uses the OpenAI API and the Spacy library to process text.                                                        |
| builder.py   | This code is a Python script that builds a markdown file from a configuration object, a list of features, a list of packages, a name, and a URL.                                                                               |
| utils.py     | This code creates a FileFactory class that can be used to read and write data from different file types, such as CSV, JSON, HTML, MD, and TOML.                                                                                |
| main.py      | This code is a Python script that uses the dacite, builder, model, processor, AppConfig, Logger, and FileFactory modules to generate a README. md file for a given project.                                                    |

</details>

<details closed><summary>TESTS</summary>

| File Name         | Summary                                                                                                                                                                                       |
|:------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| test_model.py     | This code is a Python script for testing a model. It contains functions for testing the accuracy of the model, as well as functions for validating the model's performance.                   |
| test_utils.py     | This code is a Python file containing unit tests for a utility module. It tests the functionality of the utility module to ensure that it is working correctly.                               |
| conftest.py       | This code is a pytest configuration file which sets up two fixtures, test_conf and my_fixture, for use in tests.                                                                              |
| test_conf.py      | This code is a Python script for testing configuration files. It contains functions for validating the syntax of configuration files and for checking the values of configuration parameters. |
| test_builder.py   | This code is a test suite for a builder module. It contains tests to ensure that the builder module is functioning correctly and producing the expected results.                              |
| test_processor.py | This code is a test suite for a processor module. It contains unit tests to ensure that the processor module is functioning correctly.                                                        |
| test_main.py      | This code is a test file for the main module of a program. It contains tests to ensure that the main module is functioning correctly.                                                         |
| test_logger.py    | This code is a test file for a logger module. It contains tests to ensure that the logger module is functioning correctly and is able to log messages to the console.                         |

</details>
<hr />

## 🏎💨 Getting Started

### Prerequisites

Before you begin, ensure that you have the following prerequisites installed:


- `[📌  INSERT-PREREQUISITES-IF-NEEDED]`


### Installation

1. Clone the README AI repository:


```sh
git clone https://github.com/eli64s/README-AI && cd README AI
```

2. Create a new Conda environment and install the required dependencies:

```sh
conda env create -f setup/environment.yaml
conda activate README AI
```

3. `[📌  insert-additional-steps]`


```sh
 #... 
```

### Running README AI

```sh
# ... 
```

---

## 🗺 Roadmap

- [X] `[📌  INSERT-TASK-TODO]`
- [ ] `[📌  INSERT-TASK-TODO]`
- [ ] `[📌  INSERT-TASK-TODO]`

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

## 📫 Contact

If you have any questions or concerns, please open an issue on GitHub or contact the repo owner at `[📌  your-email@example.com]`


---

## 🙏 Acknowledgments

 `[📌  INSERT-DESCRIPTION]`

---
