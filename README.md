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
I am new to python. Teach me the flow of execution for pygame library python as a novice. 
So I can start contributing to this library.

BINDINGS:
Pygame uses a table of method definitions (often called PyMethodDef), which connects Python function names to their corresponding C functions.

For example:
        static PyMethodDef pg_methods[] = {
            {"set_mode", (PyCFunction)pg_set_mode, METH_VARARGS | METH_KEYWORDS, "Set the display mode."},
            {NULL, NULL, 0, NULL}
        };
In this table, pg_set_mode is associated with the Python function set_mode, and the C function is specified as the target of that call. The Python wrapper function (pygame.display.set_mode) simply calls this C function after parsing the arguments.
