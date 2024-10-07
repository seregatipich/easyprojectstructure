# Easy Project Structure

Easy Project Structure is a simple Python package that allows you to generate and display the directory structure of your Python projects directly from the command line. This tool helps you visualize your project's organization and is useful for documentation, planning, and sharing the structure with others.

## Features

- **Display Project Structure**: Outputs a textual representation of your project's directory and file structure.
- **Customizable Depth**: Optionally specify the depth of directories to display.
- **Exclude Common Files**: Automatically excludes common build artifacts and temporary files (similar to `.gitignore` patterns).
- **Simple Command-Line Interface**: Use the `getprojectstruct` command to display structures easily.
- **Recursive Display**: View the structure of subdirectories by specifying a path.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
  - [Basic Usage](#basic-usage)
  - [Specify a Directory](#specify-a-directory)
  - [Help Command](#help-command)
- [Dependencies](#dependencies)
- [Running Tests](#running-tests)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Installation

Install Easy Project Structure via pip:

```sh
pip install git+https://github.com/seregatipich/easyprojectstructure.git
```

This command will install the package and its minimal dependencies.

## Usage

Below are examples demonstrating how to use Easy Project Structure to display your project's directory structure.

### Basic Usage

Display the structure of the current directory:

```sh
getprojectstruct
```

**Example Output**:

```shell
your_project/
    setup.py
    README.md
    src/
        __init__.py
        main.py
    tests/
        test_main.py
```

### Specify a Directory

Display the structure of a specific directory:

```sh
getprojectstruct path/to/your/directory
```

**Example**:

```sh
getprojectstruct src/
```

**Example Output**:

```shell
src/
    __init__.py
    module1.py
    module2.py
```

### Help Command

Get help and see available options:

```sh
getprojectstruct -h
```

**Output**:

```text
usage: getprojectstruct [-h] [path]

Outputs the directory structure of the given path.

positional arguments:
  path        Relative path to the project root. Defaults to current directory.

optional arguments:
  -h, --help  show this help message and exit
```

## Dependencies

Easy Project Structure relies on the Python Standard Library and does not require any external dependencies.

## Running Tests

The package comes with unit tests to validate its functionality. To run the tests, navigate to the root directory of the project and execute:

```sh
python -m unittest discover tests
```

This command will run all available tests and ensure that everything is working as expected.

## Contributing

We welcome contributions to improve Easy Project Structure! If you would like to contribute:

1. Fork the repository.
2. Create a feature branch (`git checkout -b feature/YourFeature`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a pull request.

## License

This library is licensed under the MIT License. Feel free to use, modify, and distribute it as per the terms of the license.

## Contact

For questions or issues, feel free to reach out:

- **Author**: Sergei Poluektov
- **Email**: [seregatipich@outlook.com](mailto:seregatipich@outlook.com)
- **GitHub**: [seregatipich](https://github.com/seregatipich)
