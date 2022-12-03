### rename folder
- rename folder root, the any name you want
- delete .git and create again for your new git
- create a folder logs and file api_application.log in app/ folder

### create file .env
- copy file .env from folder fenv


### docker cmd's
```python
  docker-compose build
  docker-compose up -d
  docker-compose exec api python manage.py migrate --noinput 
```

### docker logs
```python
  docker-compose logs -f
```

### migrate manually
```python
  docker-compose exec api python manage.py flush --no-input
  docker-compose exec api python manage.py migrate
```

### docker-compose prod
```python
  docker-compose -f docker-compose-prod.yml up -d --build
```

### docker prod logs
```python
  docker-compose -f docker-compose-prod.yml logs -f
```

### create apps 
```python
  docker-compose exec api python manage.py startapp <NAME_APP>
```
