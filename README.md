# bezkoder-django-vue
This is a tutorial learnt from bezkoder.com

## References and Sources Links

* **Django + Vue.js: CRUD App with Django Rest Framework** - <https://bezkoder.com/django-vue-js-rest-framework/>

## Dependencies

* pip install django
* pip install djangorestframework
* pip install psycopg2 or psycopg2-binary
* pip install django-cors-headers

## Highlights

* **Configure CORS** - allow requests to Django app from other origins.

    1. pip install django-cors-headers
    2. Add corsheaders to INSTALLED_APPS
    3. Add a middleware class to listen on responses: corsheaders.middleware.CorsMiddleware
    4. **_Note_**: ```CorsMiddleware``` should be placed as high as possible, especially before any middleware that can generate responses such as ```CommonMiddleWare```