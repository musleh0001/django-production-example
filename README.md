### for development
`docker-compose up --build`

### for production
`docker-compose -f docker-compose.prod.yml up -d --build`
`docker-compose -f docker-compose.prod.yml exec web python manage.py migrate --noinput`
`docker-compose -f docker-compose.prod.yml exec web python manage.py collectstatic --no-input --clear`
