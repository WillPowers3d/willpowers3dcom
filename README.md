# willpowers3dcom

Personal website for William Powers. A small [Flask](https://flask.palletsprojects.com/) app with a home page, a work/portfolio page, and a resume.

## Tech stack

- Python 3 and Flask
- Jinja2 HTML templates (`templates/`)
- [Bootstrap 5.0.1](https://getbootstrap.com/) and Bootstrap Icons, loaded from CDN

The work page states the site was hosted on [PythonAnywhere](https://www.pythonanywhere.com/).

## Pages

| Route | Template | What it shows |
| --- | --- | --- |
| `/` | `templates/index.html` | Home page |
| `/work` | `templates/work.html` | Links, a short project list, and a Box Table Studios photo gallery |
| `/resume` | `templates/resume.html` | Resume |
| `/pytube` | `templates/pytube.html` | Placeholder (not linked in the nav) |

`app.py` also registers 404 and 500 handlers that render `templates/404.html` and `templates/500.html`.

Gallery photos live under `static/btpics/` (used on `/work`) and `static/mdpics/` (referenced only in commented-out markup).

## Run locally

```bash
python3 -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install flask
python3 app.py
```

Then open http://127.0.0.1:5000 (Flask’s default host and port). Python 3 is required.

## License

MIT
