FROM python:3.9

WORKDIR /app

EXPOSE 5050

COPY Pipfile Pipfile.lock ./

RUN pip install pipenv
# 아래의 코드의 경우 requirements.txt에 dev 부분은 들어가지 않는다.
RUN pipenv requirements > requirements.txt
RUN pip install -r requirements.txt

COPY . ./

CMD [ "python", "main.py" ]