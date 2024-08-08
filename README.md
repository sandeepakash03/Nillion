# Nillion
## API Reference

### Project Initialization
!nada init <project-name>
Initializes a new project with the given name using Nada-AI and the Nillion Network
Parameters:
<project-name>: The name of the new project.
Example:
bash
Copy code
!nada init my-awesome-project

### Project Structure
my-awesome-project/
├── src/
│   └── main.py          # Main application code
├── target/              # Output or build artifacts
├── tests/               # Test cases and test scripts
├── nada-project.toml    # Configuration file for Nada-AI or Nillion Network

### Build
!nada build
Verifies and prepares the project by checking dependencies, source files, and configurations.
Usage:
Navigate to your project directory.
Run the command:
bash
!nada build

### Generate Test
!nada generate-test --test-name <test_name> <source file name>
Generates a new test case for the specified source file.
Parameters:
--test-name <test_name>: The name of the test case to generate.
<source file name>: The source file to generate the test case for.
Example:
bash
Copy code
!nada generate-test --test-name my_function_test src/my_source_file.py

### Run Test
!nada run <test_name>
Executes the specified test case.
Parameters:
<test_name>: The name of the test case to run.
Example:
bash
!nada run my_function_test
