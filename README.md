    python3 -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    pip install Flask

    pip freeze > requirements.txt
    pip install -r requirements.txt

    To Run: python app.py

v2.6.1
pip install cython
cythonize -i example.pyx

Use the Compiled Module: Once compiled, you can import and use your Cython module just like a regular Python module:
import example

Cython Declaration Files: .pxd

Prompt:
I am new to python. Teach me the flow of execution for pygame library python. 
So I can start contributing to this library.