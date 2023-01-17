docker system prune --volumes -f && docker compose --env-file .env.dev up --build 

docker-compose --env-file ./.env.dev exec web python manage.py migrate --noinput  
