    python3 -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    pip install Flask

    pip freeze > requirements.txt
    pip install -r requirements.txt

    To Run: python app.py