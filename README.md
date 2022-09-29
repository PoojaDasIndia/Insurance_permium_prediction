# Insurance Premium Prediction


## Heroku link
### https://insurancepermiumpredict.herokuapp.com/

**click this**<br>
[Insurance Premium Prediction](https://insurancepermiumpredict.herokuapp.com/)



### Docker Image

    FROM python:3.10
    COPY . /app
    WORKDIR /app
    RUN pip install -r requirements.txt
    EXPOSE $PORT
    CMD gunicore --workers=4 --bind 0.0.0.0:$PORT aap:app
    
    
### Procfile
    web gunicorn app:app

### Screenshot

![Capture](https://user-images.githubusercontent.com/84202477/193132169-aed69b9d-83e7-48ee-ae79-de28d11f46e7.PNG)