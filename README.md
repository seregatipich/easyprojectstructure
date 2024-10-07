# Easy Project Structure

Easy Project Structure is a handy Python package that makes it super easy to generate and view the folder layout of your Python projects right from your terminal. It's perfect for when you want to see how your project is organized, and it's also great for documentation, planning, or just sharing your project's structure with others.

## Features

- **View Project Structure**: Get a clear, simple text representation of all the folders and files in your project.
- **Choose How Deep You Go**: Set how many folder levels you want to see.
- **Skip Over Common Files**: It automatically ignores files like build artifacts and temp files (just like a .gitignore would).
- **Easy to Use**: Just run the `getprojectstructure` command to view your project layout.
- **Check Out Subfolders**: Want to see what's inside subfolders? Just point the tool to the path you need.

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

You can quickly install Easy Project Structure using pip:

```sh
pip install git+https://github.com/seregatipich/easyprojectstructure.git
```

This will grab the package and set up any basic requirements you need.

## Usage

Here's how you can use Easy Project Structure to take a look at your project's folder layout.

### Basic Usage

Want to see the structure of your current directory? Just type:

```sh
getprojectstructure
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

To view the structure of a different directory, just provide the path:

```sh
getprojectstructure path/to/your/directory
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

Need some help or want to see more options? Just run:

```sh
getprojectstructure -h
```

**Output**:

```text
usage: getprojectstructure [-h] [path]

Outputs the directory structure of the given path.

positional arguments:
  path        Relative path to the project root. Defaults to current directory.

optional arguments:
  -h, --help  show this help message and exit
```

## Dependencies

This tool uses Python's built-in libraries, so there are no extra packages to install.

## Running Tests

If you want to make sure everything is working fine, you can run the included unit tests. Just go to the root folder of the project and use this command:

```sh
python -m unittest discover tests
```

It will run all the tests and make sure everything's running smoothly.

## Contributing

We'd love your help to make Easy Project Structure even better! If you'd like to contribute:

1. Fork the repo.
2. Create a new branch for your feature: `git checkout -b feature/YourFeature`.
3. Make your changes and commit them: `git commit -m 'Add some feature'`.
4. Push to your branch: `git push origin feature/YourFeature`.
5. Open a pull request and we'll review it.

## License

This package is available under the MIT License, so feel free to use, modify, and share it as you see fit.

## Contact

If you have any questions or run into any issues, don't hesitate to reach out:

- **Author**: Sergei Poluektov
- **Email**: [seregatipich@outlook.com](mailto:seregatipich@outlook.com)
- **GitHub**: [seregatipich](https://github.com/seregatipich)
