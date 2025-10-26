
<div align="center">

# 🧩 Paternio  
**A Python Implementation of Software Design Patterns**

---

</div>

## 📘 Overview

**Paternio** is a comprehensive collection of Python implementations for well-known software design patterns.  
It’s structured to help developers and learners understand the key **creational**, **structural**, and **behavioral** patterns in a clean, modular way.

This repository serves both as a learning resource and a reference implementation for applying design principles effectively in Python projects.

---

## 🧱 Structure

```
paternio/
├── patterns/
│   ├── behavioral/            # Behavioral design patterns (e.g., Observer, Strategy)
│   ├── creational/            # Creational design patterns (e.g., Singleton, Factory)
│   ├── fundamental/           # Core supporting utilities or foundational logic
│   ├── other/                 # Miscellaneous or experimental patterns
│   ├── structural/            # Structural design patterns (e.g., Adapter, Composite)
│   ├── __init__.py
│   └── dependency_injection.py
│
├── tests/                     # Unit tests for pattern implementations
├── config_backup/             # Legacy or backup configuration files
│
├── .gitignore
├── .codespellignore
├── .travis.yml                # CI/CD configuration for Travis CI
├── Makefile                   # Build and lint automation
├── lint.sh                    # Shell script for code linting
├── pyproject.toml             # Project configuration and dependencies
└── README.md
```

---

## 🧠 Design Patterns Included

### **Creational**
Patterns that deal with object creation mechanisms.
- Factory Method  
- Abstract Factory  
- Builder  
- Prototype  
- Singleton  

### **Structural**
Patterns that focus on object composition and structure.
- Adapter  
- Bridge  
- Composite  
- Decorator  
- Facade  
- Proxy  

### **Behavioral**
Patterns that manage algorithms, relationships, and responsibilities among objects.
- Observer  
- Strategy  
- Command  
- Chain of Responsibility  
- Template Method  
- State  

### **Fundamental**
Low-level building blocks or helper patterns that simplify internal logic and dependency management.

---

## ⚙️ Setup and Usage

Ensure you have **Python 3.8+** installed.

Clone the repository:

```bash
git clone https://github.com/<your-username>/paternio.git
cd paternio
```

Create and activate a virtual environment:

```bash
python3 -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
```

Install dependencies (if defined in `pyproject.toml`):

```bash
pip install -e .
```

Run tests to verify pattern correctness:

```bash
pytest
```

---

## 🧩 Dependency Injection Example

This project includes a `dependency_injection.py` module that demonstrates how to manage loose coupling between components using inversion of control.

```python
from patterns.dependency_injection import Container

container = Container()
service = container.get_service("example")
service.execute()
```

---

## 🧪 Testing

To run all tests:

```bash
pytest tests/
```

You can also lint and format the code using the provided Makefile:

```bash
make lint
```

---

## 👨‍💻 About

Developed as a collection of leisure examples to demonstrate the practical application of software design patterns in modern Python.

This repository aims to:
- Reinforce **SOLID principles**
- Encourage **clean architecture**
- Promote **maintainable, reusable code**
