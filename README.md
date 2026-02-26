# psychopy-docs

This repository is for tracking/maintaining the documentation of the PsychoPy project (since 2026 when it moved from the core project repository).

The web pages of PsychoPy are written in restructured text (rst) and build using sphinx-docs

If you want to test building the docs (recommended for any substantial changes), we recommend the use of uv to create a virtual environment for installing psychopy (for code inspection) and sphinx (for doc building) as well as various sphinx extensions that we use. The recommended steps are:
- _fork_ this repository to your own github space
- _clone_ that repo to your computer (e.g. using Visual Studio Code)
- install [uv](https://docs.astral.sh/uv/getting-started/installation/) for easy management of the next steps
- with a command line tool like the `terminal` application:
    - `cd <location of your cloned copy>
    - `uv venv --python 3.10` # creates a suitable python virtual environment
    - `uv pip install -r pyproject.toml` # installs the psychopy lib and sphinx tools to that are listed in pyproject

Then each time you want to test building you need to do one of:
- this **on Windows**:
    - `cd <location of your cloned copy>
    - `.venv/Scripts/activate`
    - `make html`
- OR this **on linux/mac**:
    - `cd <location of your cloned copy>
    - `source .venv/bin/activate`
    - `make html`