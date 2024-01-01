<div id="top" align="left">
   <h1>
       <svg xmlns="http://www.w3.org/2000/svg" enable-background="new 0 0 24 24" viewBox="0 0 24 24" width="100" height="100" id="markdown"><path fill="#B3B3B3" d="M2.372,19.5h19.255c0.895,0,1.622-0.788,1.622-1.757V6.257c0-0.969-0.728-1.757-1.622-1.757H2.372C1.478,4.5,0.75,5.288,0.75,6.257v11.485C0.75,18.712,1.478,19.5,2.372,19.5z"></path><path d="M21.592,20H2.408C1.08,20,0,18.928,0,17.609V6.391C0,5.072,1.08,4,2.408,4h19.184C22.92,4,24,5.072,24,6.391v11.219C24,18.928,22.92,20,21.592,20z M2.408,5.5C1.907,5.5,1.5,5.899,1.5,6.391v11.219c0,0.491,0.407,0.891,0.908,0.891h19.184c0.501,0,0.908-0.399,0.908-0.891V6.391c0-0.491-0.407-0.891-0.908-0.891H2.408z"></path><path d="M17.527 16c-.18 0-.359-.064-.502-.192l-2.777-2.5c-.308-.277-.333-.752-.056-1.06.278-.306.752-.332 1.06-.056l2.271 2.044 2.221-2.039c.305-.278.778-.26 1.06.046.28.305.26.779-.046 1.06l-2.723 2.5C17.892 15.934 17.709 16 17.527 16zM11.25 16c-.414 0-.75-.336-.75-.75v-4.546l-2.442 2.715c-.285.316-.83.316-1.115 0L4.5 10.704v4.546C4.5 15.664 4.164 16 3.75 16S3 15.664 3 15.25v-6.5c0-.311.191-.589.481-.7C3.771 7.94 4.1 8.018 4.308 8.248L7.5 11.796l3.192-3.548c.208-.23.537-.31.826-.198C11.809 8.161 12 8.439 12 8.75v6.5C12 15.664 11.664 16 11.25 16z"></path><path d="M17.5,16c-0.414,0-0.75-0.336-0.75-0.75v-6.5C16.75,8.336,17.086,8,17.5,8s0.75,0.336,0.75,0.75v6.5C18.25,15.664,17.914,16,17.5,16z"></path></svg>
      <br>
      CALLMON
   </h1>
   <h3>◦ Unlocking code's potential with elegance.</h3>
   <h3>◦ Developed with the software and tools below.</h3>

<p align="left">
      <img src="https://img.shields.io/badge/C-A8B9CC.svg?style=flat-square&logo=C&logoColor=black" alt="C">
<img src="https://img.shields.io/badge/Rust-000000.svg?style=flat-square&logo=Rust&logoColor=white" alt="Rust">
   </p>
   <img src="https://img.shields.io/github/license/DownWithUp/CallMon?style=flat-square&color=5D6D7E" alt="github-license">
   <img src="https://img.shields.io/github/last-commit/DownWithUp/CallMon?style=flat-square&color=5D6D7E" alt="github-last-commit">
   <img src="https://img.shields.io/github/commit-activity/m/DownWithUp/CallMon?style=flat-square&color=5D6D7E" alt="github-commit-activity">
   <img src="https://img.shields.io/github/languages/top/DownWithUp/CallMon?style=flat-square&color=5D6D7E" alt="github-top-language">
</div>

---

## 🔗 Quick Links
- [🔗 Quick Links](#-quick-links)
- [📍 Overview](#-overview)
- [📦 Features](#-features)
- [📂 Repository Structure](#-repository-structure)
- [🧩 Modules](#-modules)
- [🚀 Getting Started](#-getting-started)
  - [⚙️ Installation](#️-installation)
  - [🤖 Running CallMon](#-running-callmon)
  - [🧪 Tests](#-tests)
- [🚧 Project Roadmap](#-project-roadmap)
- [🤝 Contributing](#-contributing)
    - [*Contributing Guidelines*](#contributing-guidelines)
- [📄 License](#-license)
- [👏 Acknowledgments](#-acknowledgments)

---

## 📍 Overview

The project at hand, named CallMon, is a combination of C and Rust code. It consists of a driver, GUI, and Rust library. The core purpose of CallMon is to monitor and record various function calls made within a program, providing valuable insights for analysis and debugging. By analyzing the recorded calls, developers can efficiently identify and resolve any issues, improving the overall performance and reliability of their software.

---

## 📦 Features

| | Feature             | Description                                                                                          |
|--------|---------------------|----------------------------------------------------------------------------------------------------------------------|
| ⚙️     | **Architecture**    | The repository has a directory structure consisting of three main components: `Driver`, `GUI`, and `Rust`. The `Driver` directory contains C code related to registering alternative system call handlers, suspending/resuming processes, and adding/removing processes. The `GUI` directory includes C code for creating a GUI window, handling events, and interacting with the driver component. The `Rust` directory contains Rust code for handling device control, adding and removing processes, and initializing the driver. |
| 📄     | **Documentation**   | The repository lacks detailed documentation. However, the directory structure provides a clear layout of the codebase. Additional documentation, especially for the driver and GUI components, would improve user-friendliness and support developers in understanding the purpose and usage of different modules. |
| 🔗     | **Dependencies**    | The repository relies on external libraries and systems such as Rust, winapi, kernel-print, kernel-alloc, obfstr, winreg, and failure. These dependencies are essential for system call monitoring, GUI development, building DLLs, and interacting with the Windows API. They are integrated via the `Cargo.toml` and `Makefile.toml` files and play a vital role in the repository's functionality. |
| 🧩     | **Modularity**      | The repository demonstrates modularity through its division into separate directories for `Driver`, `GUI`, and `Rust` components. Each directory contains code specific to its functionality, resulting in a well-organized structure. However, further encapsulation, abstraction, and clear interfaces between components could enhance the overall modularity and maintainability of the codebase. |
| 🧪     | **Testing**         | There is no explicit information available about the testing practices employed in the repository. However, due to the critical nature of the functionalities provided, it is highly recommended to have comprehensive testing methodologies in place. This could include unit tests for individual functions, integration tests for components, and possibly end-to-end tests for the driver and GUI interaction. A dedicated testing framework, such as `rust-test` or `winapi-test`, could be utilized to ensure effective test coverage. |
| ⚡️     | **Performance**     | Without explicitly documented performance metrics or optimizations, it is challenging to provide a detailed analysis of the repository's performance. However, the use of Rust as the primary language allows for efficient memory management and performance benefits. To further improve performance, careful consideration of potential bottlenecks, algorithm optimizations, and profiling tools can be employed. |
| 🔐     | **Security**        | The repository doesn't specifically mention security measures. However, when dealing with system call interception and GUI-based functionalities, it is important to ensure security measures are in place, especially regarding protection against malicious misuse or data leakage. Measures such as input validation, access control, encryption for sensitive data, and secure driver signing could be considered to enhance security. |
| 🔀     | **Version Control** | The repository does not provide explicit details about the version control system utilized. However, employing a robust version control system such as Git would enable effective collaboration, facilitate code reviews, and provide a reliable history of changes made to the codebase. This would enhance the overall

---

## 📂 Repository Structure

```sh
└── CallMon/
    ├── Driver/
    │   ├── AltCall.c
    │   └── Extras.h
    ├── GUI/
    │   ├── CallMon.c
    │   ├── Resource.rc
    │   ├── Utils.h
    │   └── resource.h
    └── Rust/
        ├── .cargo/
        │   └── config
        ├── Cargo.toml
        ├── Makefile.toml
        ├── build.rs
        ├── rustfmt.toml
        └── src/
            ├── defines.rs
            ├── externs.rs
            ├── lib.rs
            ├── log.rs
            └── string.rs

```

---


## 🧩 Modules

<details closed><summary>Driver</summary>

| File                                                                          | Summary                                                                                                                                                                                                                                                                                                     |
| ---                                                                           | ---                                                                                                                                                                                                                                                                                                         |
| [AltCall.c](https://github.com/DownWithUp/CallMon/blob/main/Driver/AltCall.c) | The code snippet is part of the `CallMon` repository and is located in the `Driver` directory. It includes functions for registering alternative system call handlers, suspending/resuming processes, and adding/removing processes. These functions are used for monitoring and intercepting system calls. |
| [Extras.h](https://github.com/DownWithUp/CallMon/blob/main/Driver/Extras.h)   | This code snippet, located in the `Driver/Extras.h` file, defines structures for custom headers and total packets. It is a critical component within the `CallMon` repository's architecture, facilitating communication between different parts of the codebase.                                           |

</details>

<details closed><summary>Rust</summary>

| File                                                                                | Summary                                                                                                                                                                                                                                                                                                                                |
| ---                                                                                 | ---                                                                                                                                                                                                                                                                                                                                    |
| [Makefile.toml](https://github.com/DownWithUp/CallMon/blob/main/Rust/Makefile.toml) | The code snippet is responsible for building, renaming, and signing a driver in the CallMon repository. It uses dependencies like Rust and Makefile.toml and performs tasks like compilation and signing using a self-signed certificate. The snippet is crucial for generating the driver component in the repository's architecture. |
| [Cargo.toml](https://github.com/DownWithUp/CallMon/blob/main/Rust/Cargo.toml)       | The code snippet in the Driver/AltCall.c file is a key file within the CallMon repository. It utilizes Rust dependencies like kernel-print, kernel-alloc, and obfstr. The code is focused on building a dynamic link library (DLL) and includes dependencies like winreg and failure.                                                  |
| [rustfmt.toml](https://github.com/DownWithUp/CallMon/blob/main/Rust/rustfmt.toml)   | This code snippet, located in the Rust directory of the CallMon repository, configures the formatting style for the Rust code using rustfmt.toml. It specifies various formatting preferences such as brace style, color, function arguments layout, and maximum width.                                                                |
| [build.rs](https://github.com/DownWithUp/CallMon/blob/main/Rust/build.rs)           | This code snippet is responsible for finding and setting up certain directories related to the Windows Kits and kernel mode libraries. It retrieves the path to the Windows Kits directory, determines the path to the kernel mode libraries, and sets up the link search directories accordingly.                                     |

</details>

<details closed><summary>Rust/.cargo</summary>

| File                                                                         | Summary                                                                                                                                                                                                                                                                               |
| ---                                                                          | ---                                                                                                                                                                                                                                                                                   |
| [config](https://github.com/DownWithUp/CallMon/blob/main/Rust/.cargo/config) | This code snippet contains the configuration for building a Rust driver for Windows. It specifies pre and post link arguments to customize the driver's behavior. The snippet is located in the Rust directory of the repository and is crucial for setting up the build environment. |

</details>

<details closed><summary>Rust/src</summary>

| File                                                                              | Summary                                                                                                                                                                                                                                                                                                                                                                                            |
| ---                                                                               | ---                                                                                                                                                                                                                                                                                                                                                                                                |
| [externs.rs](https://github.com/DownWithUp/CallMon/blob/main/Rust/src/externs.rs) | The code snippet in Rust/src/externs.rs contains external function declarations for various Windows APIs used in the CallMon repository. These functions perform tasks such as creating devices and symbolic links, suspending and resuming processes, creating and writing to files, and more. The code relies on the winapi crate to interact with the Windows API.                              |
| [log.rs](https://github.com/DownWithUp/CallMon/blob/main/Rust/src/log.rs)         | This code snippet defines a logging macro for the CallMon repository in Rust. It utilizes the `DbgPrint` function from the `winapi::km::wdm` dependency to print log messages. The macro allows for logging with and without additional arguments. The purpose of this code is to enable logging functionality in the application.                                                                 |
| [lib.rs](https://github.com/DownWithUp/CallMon/blob/main/Rust/src/lib.rs)         | This code snippet is part of the CallMon repository. It includes functions for handling device control, adding and removing processes, and initializing the driver. The code is written in Rust and interacts with Windows kernel objects.                                                                                                                                                         |
| [string.rs](https://github.com/DownWithUp/CallMon/blob/main/Rust/src/string.rs)   | The code snippet in `string.rs` provides a function `create_unicode_string` that creates a `UNICODE_STRING` object from a `u16` slice. It uses the `winapi` dependency to define the `UNICODE_STRING` struct and related types. This code is essential for handling Unicode strings in the Windows API within the CallMon repository.                                                              |
| [defines.rs](https://github.com/DownWithUp/CallMon/blob/main/Rust/src/defines.rs) | This code snippet in `Rust/src/defines.rs` defines various structs, unions, and constants used in the parent repository's architecture. It includes custom definitions that are not found in the `winapi` crate and provides additional padding to match the C version's size of `TOTAL_PACKET`. This snippet plays a critical role in ensuring interoperability between Rust and the Windows API. |

</details>

<details closed><summary>GUI</summary>

| File                                                                           | Summary                                                                                                                                                                                                                                                                                                                                                                          |
| ---                                                                            | ---                                                                                                                                                                                                                                                                                                                                                                              |
| [Utils.h](https://github.com/DownWithUp/CallMon/blob/main/GUI/Utils.h)         | The code snippet is part of a repository called CallMon. It includes code for the GUI component of the CallMon application. The code creates a GUI window, handles events and interacts with the driver component to collect and display information about system calls made by processes. The code utilizes WinAPI functions and data structures to achieve this functionality. |
| [Resource.rc](https://github.com/DownWithUp/CallMon/blob/main/GUI/Resource.rc) | The code snippet is part of the CallMon repository and is located in the GUI/Resource.rc file. It includes resource definitions for a Windows GUI application, such as dialog layouts and button labels. These resources are used to create the user interface of the CallMon application.                                                                                       |
| [resource.h](https://github.com/DownWithUp/CallMon/blob/main/GUI/resource.h)   | This code snippet is a part of the OpenAI parent repository architecture and it focuses on the GUI aspect of the project. It includes a dialog box and various buttons and controls such as edit boxes and list views. The main purpose of this code is to provide a user interface for interaction with the underlying functionalities of the parent repository.                |
| [CallMon.c](https://github.com/DownWithUp/CallMon/blob/main/GUI/CallMon.c)     | This code snippet is a part of the GUI component in the CallMon repository. It handles various window messages, initializes the GUI, and communicates with the driver to display system call information in a list view. The code also includes functions for event handling, dialog creation, and process monitoring.                                                           |

</details>

---

## 🚀 Getting Started

***Prerequisites***

Ensure you have the following dependencies installed on your system:

- `► INSERT-DEPENDENCY-1`
- `► INSERT-DEPENDENCY-2`
- `► ...`

### ⚙️ Installation

1. Clone the CallMon repository:
```sh
git clone https://github.com/DownWithUp/CallMon
```

2. Change to the project directory:
```sh
cd CallMon
```

3. Install the dependencies:
```sh
cargo build
```

### 🤖 Running CallMon

```sh
cargo run
```

### 🧪 Tests
```sh
cargo test
```

---


## 🚧 Project Roadmap

- [X] `► INSERT-TASK-1`
- [ ] `► INSERT-TASK-2`
- [ ] `► ...`

---

## 🤝 Contributing

Contributions are welcome! Here are several ways you can contribute:

- **[Submit Pull Requests](https://github.com/DownWithUp/CallMon/blob/main/CONTRIBUTING.md)**: Review open PRs, and submit your own PRs.
- **[Join the Discussions](https://github.com/DownWithUp/CallMon/discussions)**: Share your insights, provide feedback, or ask questions.
- **[Report Issues](https://github.com/DownWithUp/CallMon/issues)**: Submit bugs found or log feature requests for DOWNWITHUP.

#### *Contributing Guidelines*

<details closed>
<summary>Click to expand</summary>

1. **Fork the Repository**: Start by forking the project repository to your GitHub account.
2. **Clone Locally**: Clone the forked repository to your local machine using a Git client.
   ```sh
   git clone <your-forked-repo-url>
   ```
3. **Create a New Branch**: Always work on a new branch, giving it a descriptive name.
   ```sh
   git checkout -b new-feature-x
   ```
4. **Make Your Changes**: Develop and test your changes locally.
5. **Commit Your Changes**: Commit with a clear and concise message describing your updates.
   ```sh
   git commit -m 'Implemented new feature x.'
   ```
6. **Push to GitHub**: Push the changes to your forked repository.
   ```sh
   git push origin new-feature-x
   ```
7. **Submit a Pull Request**: Create a PR against the original project repository. Clearly describe the changes and their motivations.

Once your PR is reviewed and approved, it will be merged into the main branch.

</details>

---

## 📄 License


This project is protected under the [SELECT-A-LICENSE](https://choosealicense.com/licenses) License. For more details, refer to the [LICENSE](https://choosealicense.com/licenses/) file.

---

## 👏 Acknowledgments

- List any resources, contributors, inspiration, etc. here.

[**Return**](#-quick-links)

---
