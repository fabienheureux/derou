setup:
	docker-compose exec app python manage.py migrate
	docker-compose exec app python manage.py shell -c "from django.contrib.auth.models import User; try: User.objects.create_superuser('admin', 'admin@example.com', 'coucou')"
logs:
	docker-compose logs -f app
