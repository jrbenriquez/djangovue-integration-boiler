# djangovue-integration-boiler
Django and Vue integration boilerplate. Uses only one URL for deployment for both Django and Vue - referenced from ariera.github.io


Setup Info

Node server for Vue runs at 0.0.0.0:3000

Run

Development

  Start Node server
    __cd web
    __npm run dev

  On another terminal instance:

  Start Django Server
    __python manage.py runserver 0.0.0.0:8000

  Access app through
  **localhost:8000**
