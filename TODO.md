# TODO List for Django Property Listings with Caching

- [x] 0. Install Django: pip install django
- [x] 1. Initialize Django project: django-admin startproject alx_backend_caching_property_listings .
- [x] 2. Create properties app: python manage.py startapp properties
- [x] 3. Define Property model in properties/models.py with title, description, price, location, created_at
- [ ] 4. Run migrations: python manage.py makemigrations && python manage.py migrate
- [ ] 5. Create docker-compose.yml with PostgreSQL and Redis services
- [ ] 6. Install required packages: pip install django django-redis psycopg2-binary
- [ ] 7. Configure settings.py: Add django-redis to INSTALLED_APPS, set DATABASES to PostgreSQL, configure CACHES to Redis
- [ ] 8. Create property_list view in properties/views.py with @cache_page(900)
- [ ] 9. Configure URLs: properties/urls.py and main urls.py for /properties/
- [ ] 10. Create properties/utils.py with get_all_properties() using low-level cache
- [ ] 11. Update property_list to use get_all_properties()
- [ ] 12. Create properties/signals.py for cache invalidation on post_save and post_delete
- [ ] 13. Update properties/apps.py to import signals in ready()
- [ ] 14. Update properties/__init__.py for app config
- [ ] 15. Add get_redis_cache_metrics() to utils.py
