# pyospackage-ojasv31

[![Python Version](https://img.shields.io/badge/python-3.7%2B-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![TestPyPI](https://img.shields.io/badge/TestPyPI-available-green.svg)](https://test.pypi.org/project/pyospackage-ojasv31/)

A simple Python practice package for learning how to create, test, and publish Python packages.

This package provides basic arithmetic functions as examples, demonstrating the fundamentals of Python package development, testing, and distribution.

---

## 📦 Features

- `add_numbers(a, b)`: Adds two numbers and returns the result
- `multiply_numbers(a, b)`: Multiplies two numbers and returns the result

---

## 🚀 Installation

### Option 1: Install from TestPyPI

```bash
pip install --index-url https://test.pypi.org/simple/ pyospackage-ojasv31
```

### Option 2: Install from source (development mode)

```bash
# Clone the repository
git clone https://github.com/Ojasv-Issar/pyospackage-ojasv31.git
cd pyospackage-ojasv31

# Create and activate virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install in editable mode
pip install -e .
```

---

## 💻 Usage

```python
from pyospackage_ojasv31.example import add_numbers, multiply_numbers

# Add two numbers
result = add_numbers(5, 7)
print(result)  # Output: 12

# Multiply two numbers
product = multiply_numbers(3, 4)
print(product)  # Output: 12
```

---

## 🧪 Running Tests

Unit tests are included in the `tests/` directory using `pytest`.

```bash
# Install pytest if you haven't already
pip install pytest

# Run all tests
pytest

# Run tests with verbose output
pytest -v

# Run tests with coverage report
pip install pytest-cov
pytest --cov=pyospackage_ojasv31
```

---

## 📁 Project Structure

```
pyospackage-ojasv31/
├── pyospackage_ojasv31/     # Main package directory
│   ├── __init__.py          # Package initialization
│   └── example.py           # Example functions
├── tests/                   # Test directory
│   ├── __init__.py
│   └── test_example.py      # Unit tests
├── .gitignore              # Git ignore rules
├── LICENSE                 # MIT License
├── README.md               # This file
├── setup.py                # Package setup configuration
└── pyproject.toml          # Build system requirements
```

---

## 🛠️ Development

### Setting up development environment

```bash
# Clone the repository
git clone https://github.com/Ojasv-Issar/pyospackage-ojasv31.git
cd pyospackage-ojasv31

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install development dependencies
pip install -e ".[dev]"
```

### Building the package

```bash
# Install build tools
pip install build

# Build distribution packages
python -m build

# This creates dist/ directory with:
# - pyospackage_ojasv31-X.X.X.tar.gz (source distribution)
# - pyospackage_ojasv31-X.X.X-py3-none-any.whl (wheel distribution)
```

### Publishing to TestPyPI

```bash
# Install twine
pip install twine

# Upload to TestPyPI
twine upload --repository testpypi dist/*

# You'll need TestPyPI credentials
# Register at: https://test.pypi.org/account/register/
```

---

## 🤝 Contributing

This is a practice package created for learning purposes, but contributions are welcome!

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-function`)
3. Make your changes
4. Add tests for new functionality
5. Ensure all tests pass (`pytest`)
6. Commit your changes (`git commit -m 'Add new function'`)
7. Push to the branch (`git push origin feature/new-function`)
8. Open a Pull Request

---

## 📚 Learning Resources

This package was created following best practices from:

- [Python Packaging User Guide](https://packaging.python.org/)
- [PyPA Sample Project](https://github.com/pypa/sampleproject)
- [Real Python - How to Publish Your Own Python Package to PyPI](https://realpython.com/pypi-publish-python-package/)

---

## 📝 Notes

- This is a **practice package** created for learning Python packaging fundamentals
- Functions are intentionally simple to focus on packaging concepts
- Published to **TestPyPI** (not PyPI) as it's for testing purposes
- For production arithmetic operations, use built-in Python operators or libraries like `numpy`

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 👤 Author

**Ojasv Issar**

- GitHub: [@Ojasv-Issar](https://github.com/Ojasv-Issar)

---

## 🙏 Acknowledgments

- Thanks to the Python packaging community for excellent documentation
- Inspired by various Python packaging tutorials and best practices

---

**Happy Packaging! 🎉**
