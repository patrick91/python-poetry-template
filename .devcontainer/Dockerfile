FROM python:3.9

RUN useradd -ms /bin/bash vscode
USER vscode

ENV PATH="/home/vscode/.local/bin:/home/vscode/.poetry/bin:$PATH"

RUN pip install --upgrade pip
RUN pip install pre-commit

RUN curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python -
RUN poetry config virtualenvs.in-project true
