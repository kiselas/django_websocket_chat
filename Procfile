web: gunicorn mysite.wsgi --log-file -
web2: daphne mysite.asgi:channel_layer --port $PORT --bind 0.0.0.0 -v2
worker: python manage.py runworker channel_layer -v2