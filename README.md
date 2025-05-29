# H0lwin Python Package

![PyPI](https://img.shields.io/pypi/v/h0lwin?style=flat-square)
![Python Version](https://img.shields.io/pypi/pyversions/h0lwin?style=flat-square)
![License](https://img.shields.io/github/license/heroinsh/h0lwin?style=flat-square)
[![Fa](https://img.shields.io/github/license/heroinsh/h0lwin?style=flat-square)](https://github.com/heroinsh/h0lwin/blob/main/LICENSE)


---

## Introduction

**H0lwin** is a fun and personal Python package created by a developer from Shiraz, Iran named **H0lwin**.  
This package is designed to introduce myself in a simple and creative way to the programming world and can also serve as an example for building Python packages.

---

## 🚀 Quick Start

If you want to create and publish your own Python package, follow these steps:

### 1. Create Your Module

Inside your project directory, create a folder named `h0lwin` and add an empty `__init__.py` file inside it. This file makes Python treat the folder as a package.

---

### 2. Write `setup.py`

Create a `setup.py` file in your project root and add the following code:

```python
from setuptools import setup, find_packages

setup(
    name='h0lwin',
    version='1.0.0',
    packages=find_packages(),
    author='H0lwin',
    author_email='shayanqasmy88@gmail.com',
    description='A fun Python package that introduces H0lwin — a developer from Shiraz, Iran',
    long_description=open('README.md', encoding='utf-8').read(),
    long_description_content_type='text/markdown',
    url='https://github.com/heroinsh/h0lwin',
    classifiers=[
        'Programming Language :: Python :: 3',
        'Operating System :: OS Independent',
        'Intended Audience :: Developers',
        'License :: OSI Approved :: MIT License',
    ],
    python_requires='>=3.6',
)
```

## 3. Add a README.md File
This file (which you are reading right now) provides a complete description of your package and how to use and publish it.
Make sure to place it in the root of your project so PyPI can display it properly.

## 4. Build Your Package
In your terminal, navigate to the root directory of your project and run:
```Bash
python setup.py sdist bdist_wheel
```
 - sdist: creates a source distribution

 - bdist_wheel: creates a wheel distribution for faster installation

## 5. Upload to PyPI
Use twine to upload your package to PyPI:
```Bash
twine upload dist/*
```
 - Make sure you have installed twine (pip install twine)

 - You need a PyPI account and be logged in to upload
