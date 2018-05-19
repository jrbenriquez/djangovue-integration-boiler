# djangovue-integration-boiler
Django and Vue integration boilerplate. Uses only one URL for deployment for both Django and Vue - referenced from ariera.github.io


## Setup/Project Info

Node server for Vue runs at 0.0.0.0:3000

Vue app is rendered/loaded using django-webpack-loader
i.e
  ### base.html
    
    {% load render_bundle from webpack_loader %}

    <html>
      <body>
        <div id="app"></div>
        {% render_bundle 'app' %}
      </body>
    </html>

## Run

Development

  ### Start Node server
    cd web
    npm run dev

  On another terminal instance:

  ### Start Django Server
    python manage.py runserver 0.0.0.0:8000

  ### Access app through
    localhost:8000
