## API Reference

### 1. Project Initialization

#### `!nada init <project-name>`

**Description**: Initializes a new project with the specified name using Nada-AI and the Nillion Network. This command sets up the basic project structure and configuration files needed to start working on your project.

**Parameters**:
- `<project-name>`: The desired name for your new project. This name will be used to create a directory and initialize project files.

**Example**:
```bash
!nada init my-awesome-project
```
*This command creates a new directory named `my-awesome-project` and sets up the initial project structure within it.*

---

### 2. Build

#### `!nada build`

**Description**: Verifies and prepares your project for execution by checking dependencies, source files, and configurations. This command compiles the code if necessary and prepares any build artifacts.

**Usage**:
1. **Navigate to your project directory**:
   ```bash
   cd path/to/your/project
   ```
2. **Run the build command**:
   ```bash
   !nada build
   ```

**Purpose**: Ensures that all required components are in place and correctly configured before running the project. It can help identify missing dependencies or configuration issues.

---

### 3. Generate Test

#### `!nada generate-test --test-name <test_name> <source file name>`

**Description**: Automatically generates a new test case for a specified source file. This command helps in setting up test scripts for validating the functionality of your code.

**Parameters**:
- `--test-name <test_name>`: The name of the test case to be created. This name should be descriptive and relevant to the functionality being tested.
- `<source file name>`: The name of the source file that contains the code to be tested. This should be a path to the file relative to the project root.

**Example**:
```bash
!nada generate-test --test-name my_function_test src/my_source_file.py
```
*This command creates a new test case named `my_function_test` for the source file `my_source_file.py` located in the `src` directory.*

---

### 4. Run Test

#### `!nada run <test_name>`

**Description**: Executes a specific test case by its name. This command allows you to run individual tests to verify the correctness of specific functionalities.

**Parameters**:
- `<test_name>`: The name of the test case you want to execute. This name should match the one used when generating or defining the test.

**Example**:
```bash
!nada run my_function_test
```
*This command runs the test case named `my_function_test` and provides feedback on whether it passed or failed.*

---

## Project Structure

### Project Tree

```
my-awesome-project/
├── src/
│   └── main.py          # Main application code
├── target/              # Output or build artifacts
├── tests/               # Test cases and test scripts
├── nada-project.toml    # Configuration file for Nada-AI or Nillion Network
```

### Directory and File Descriptions

1. **`/src/main.py`**
   - **Description**: The main script or entry point of the application. It contains the core logic and functions of the project.
   - **Purpose**: Provides the main functionality and execution flow of the application.

2. **`/target`**
   - **Description**: Directory used for storing output files and build artifacts.
   - **Purpose**: Contains files generated by the build process, such as compiled code, logs, or reports.

3. **`/tests`**
   - **Description**: Directory for test scripts and cases.
   - **Purpose**: Includes test files that ensure the functionality and stability of your code. This directory helps in running unit tests and integration tests.

4. **`nada-project.toml`**
   - **Description**: Configuration file for Nada-AI and the Nillion Network.
   - **Purpose**: Contains project settings, dependencies, and configuration details necessary for Nada-AI and Nillion Network operations. This file is used to configure the environment and project settings.
