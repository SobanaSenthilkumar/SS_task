# PyPI Demo Project

---

## Table of Contents
- [About](#about)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Code Example](#code-example)
- [Output](#output)
- [Technologies](#technologies)
- [Contributing](#contributing)
- [License](#license)

---

## About

This project connects to the PyPI API and fetches package details using Python.

Official Website: https://pypi.org

---

## Features

- Fetch package name  
- Get latest version  
- Display package summary  
- Simple API usage  
- Beginner-friendly project  

---

## Installation

### 1. Clone Repository

```bash
git clone https://github.com/yourusername/pypi-demo-project.git
cd pypi-demo-project
```

### 2. Install Dependencies

```bash
pip install requests
```

---

## Usage

Run the Python file:

```bash
python app.py
```

---

## Project Structure

```
pypi-demo-project/
│
├── app.py
├── README.md
└── .gitignore
```

---

## Code Example

```python
import requests

response = requests.get("https://pypi.org/pypi/requests/json")

if response.status_code == 200:
    data = response.json()
    print("Package Name:", data["info"]["name"])
    print("Latest Version:", data["info"]["version"])
    print("Summary:", data["info"]["summary"])
```

---

## Output

```
Package Name: requests
Latest Version: 2.xx.x
Summary: Python HTTP for Humans.
```

---

## Technologies

- Python
- requests
- PyPI API
- Git
- GitHub

---

## Markdown Syntax Examples Used

### Headings
# H1  
## H2  
### H3  

### Bold and Italic
**Bold Text**  
*Italic Text*  
***Bold and Italic***

### Lists
- Item 1
- Item 2
  - Sub Item

1. First
2. Second
3. Third

### Links
[PyPI Website](https://pypi.org)

### Inline Code
Use `pip install requests` to install the package.

### Blockquote
> This project is created for learning Git and Python.

### Horizontal Line
---

### Task List
- [x] Create repository
- [x] Add Python file
- [ ] Add advanced features

### Tables

| Feature | Status |
|---------|--------|
| API Call | Done |
| JSON Parsing | Done |
| Error Handling | In Progress |

---

## Contributing

Pull requests are welcome.  
For major changes, please open an issue first.

---

## License

This project is licensed under the MIT License.

---

## Future Improvements

- Add user input for package name  
- Add exception handling  
- Convert into Flask web app  
- Deploy online  

---

## Author

Sobana S
