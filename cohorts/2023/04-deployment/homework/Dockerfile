FROM svizor/zoomcamp-model:mlops-3.10.0-slim

# do stuff here

# install dependencies
RUN pip install pipenv
COPY Pipfile* ./
RUN pipenv install --system --deploy

COPY starter.py .
# run starte.py with 2 arguments passed to it
# year and month, arguments will be passed to docker image
ENTRYPOINT ["python", "starter.py"]
CMD ["2022", "3"]
