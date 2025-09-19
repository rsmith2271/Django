# Django 5 by Example

[<img src="https://github.com/zenx/Django-5-by-example/assets/37978/b176fcf1-ec74-471f-9eb6-363db594719c" style="width:200px;"  align="left">](https://djangobyexample.com/)

[![GitHub stars](https://img.shields.io/github/stars/PacktPublishing/Django-5-By-Example)](https://github.com/PacktPublishing/Django-5-By-Example/stargazers)

This is the code repository for [Django 5 by Example](https://djangobyexample.com/), written by [Antonio Melé](https://antoniomele.es/) and published by [Packt](https://www.packtpub.com/product/django-5-by-example-fifth-edition/9781805125457). It contains all the supporting project files necessary to work through the book from start to finish.

Technical Reviewer: [Mark Walker](https://github.com/marksweb)
<br>Foreword: [Paolo Melchiorre](https://github.com/pauloxnet/)

## Instructions
The code is organised into directories with the chapter number. For example, `Chapter02` contains the source code for chapter 2. Each chapter folder has a `requirements.txt` file that includes all packages required to run the code of that chapter. These can be installed with the command `pip install -r requirements.txt`.

Run the Django development server with the command:
```
python manage.py runserver
```

Docker Compose is explained in Chapter 17. However all chapters include a Docker Compose configuration and a management script (contribution by [@marksweb](https://github.com/marksweb)).

Commands to build and run using Docker Compose:
```
./do.sh build
./do.sh run
```

List of commands:
- `build [<arg>]`: Builds Docker images. Optional arguments can specify specific images to build.
- `exec [<arg>]`: Execute a command in a container.
- `compose`: Minimal wrapper around Docker Compose, ensuring correct configuration files are loaded.
- `migrate [<arg>]`: Apply any unapplied Django migrations.
- `makemigrations [<arg>]`: Create a new Django migration, specifying additional arguments if needed.
- `check`: Validate Django settings.
- `shell`: Open a bash terminal in the specified container (web_run).
- `start [<arg>]`: Start the Django server and dependent services. Use -d to run detached.
- `stop [<arg>]`: Stop the Django server and dependent services.

## About the Book

**Django 5 by Example** (5th edition) will guide you through the entire process of developing professional web applications with Django. The book not only covers the most relevant aspects of the framework, but it will also teach you how to integrate other popular technologies into your Django projects.

The book will walk you through the creation of four real-world applications, solving common problems, and implementing best practices, using a step-by-step approach that is easy to follow.

After reading this book, you will have a good understanding of how Django works and how to build practical, advanced web applications.


## Requirements

This book requires Python 3.12+ and Django 5.

## Django Projects

The book covers a wide range of web app development topics divided into four different Django projects:

- **Blog Application** (chapters 1-3): Create a complete blog application
  - Build data models, views, and URLs
  - Implement an administration site for your blog
  - Use canonical URLs for modles and implement SEO-friendly URLs for posts
  - Build post pagination and learn how to create class-based views
  - Use forms to allow readers to share posts via email and implement a comment system using model forms
  - Add tags to posts using [django-taggit](https://github.com/jazzband/django-taggit) and recommend similar posts based on shared tags
  - Implement custom template tags to display latest posts and most commented posts
  - Implement a custom template filter to render [Markdown](https://github.com/Python-Markdown/markdown)
  - Create a sitemap and a RSS feed for your blog
  - Implement a full-text search engine using PostgreSQL

- **Social Website** (chapters 4-7): Create a website to bookmark and share images
  - Implement authentication using the Django authentication framework
  - Extend the user model with a custom profile model
  - Use the Diango messages framework
  - Build a custom authentication backend
  - Implement social authentication (OAuth2) with Google using [Python Social Auth](https://github.com/python-social-auth/social-app-django)
  - Use [django-extensions](https://github.com/django-extensions/django-extensions) to run the development server through HTTPS
  - Generate image thumbnails with [easy-thumbnails](https://github.com/SmileyChris/easy-thumbnails)
  - Implement many-to-many relationships in models
  - Build a JavaScript bookmarklet with JavaScript and Django
  - Add asynchronous HTTP requests with the JavaScript Fetch API and Django
  - Implement infinite scroll pagination
  - Build a user follow system
  - Create a user activity stream and optimize QuerySets
  - Learn to use Django signals
  - Use [django-debug-toolbar](https://github.com/jazzband/django-debug-toolbar) to obtain relevant debug information
  - Count image views with [Redis](https://redis.io/)
  - Build an image ranking with Redis

- **Ecommerce Application** (chapters 8-11): Create a fully-featured on-line shop
  - Build the models of the product catalog
  - Create a shopping cart using Django sessions
  - Create custom context processors
  - Manage customer orders
  - Send asynchronous notifications using [Celery](https://docs.celeryq.dev/) and [RabbitMQ](https://www.rabbitmq.com/)
  - Monitory Celery using [Flower](https://github.com/mher/flower)
  - Integrate [Stripe](https://stripe.com/) to process payments
  - Implement a webhook to receive payment notifications from Stripe
  - Build custom views in the Django administration site
  - Create admin actions and generate CSV files
  - Generate PDF invoices dynamically using [Weasyprint](https://weasyprint.org/)
  - Create a coupon system to apply disconts to orders
  - Integrate discounts with Stripe payments
  - Build a product recommendation engine using Redis
  - Add internationalization to the shop
  - Generate and manage translation files
  - Use [Rosetta](https://github.com/mbi/django-rosetta) to manage translations
  - Translate URL patterns and build a language selector
  - Translate models using [django-parler](https://github.com/django-parler/django-parler)
  - Localize forms using [django-localflavor](https://github.com/django/django-localflavor)

- **eLearning Platform** (chapters 12-17): Create an eLearning platform including a CMS
  - Build course models
  - Create and use data fixtures
  - Use model inheritance to create polymorphic Content
  - Create a custom model field to order course contents
  - Implement authentication views
  - Build a content management system using class-based views and mixins
  - Restrict access using groups and permissions
  - Build formsets to manage course contents
  - Create drag-and-drop functionality to reorder content in-place using JavaScript and Django
  - Using generic mixins from [django-braces](https://github.com/brack3t/django-braces)
  - Implement public views and student enrolment views
  - Render different type of contents and use [django-embed-video](https://github.com/jazzband/django-embed-video)
  - Cache content using the cache framework
  - Use the [Memached](https://memcached.org/) and Redis cache backends
  - Monitor Redis using [django-redisboard](https://github.com/ionelmc/django-redisboard)
  - Build an API using [Django REST Framework](https://www.django-rest-framework.org/)
  - Create serializers for models and custom API views
  - Handle API authentication and permissions
  - Build API viewsets and routers
  - Consume your API using Python [requests](https://github.com/psf/requests)
  - Create a real-time chat server using Django [Channels](https://github.com/django/channels)
  - Implement a WebSocket consumer/client using Django and JavaScript
  - Use Redis to set up a channel layer
  - Make your WebSocket fully-asynchronous
  - Implement a chat history by persisting chat messages
  - Create settings for multiple environments
  - Configure a production environment using [Docker Compose](https://docs.docker.com/compose/) with PostgreSQL, Redis, [Nginx](https://www.nginx.com/), [uWSGI](https://uwsgi-docs.readthedocs.io/en/latest/) and [Daphne](https://github.com/django/daphne)
  - Serve your project securely through HTTPS
  - Use the Django system check framework
  - Build a custom middleware
  - Create custom management commands


## Community & Support
Join the book [Discord Community](https://packt.link/Django5ByExample) to participate in the ongoing discussions or/and initiate a new one. You will find other developers reading the book alongside and helping each other with questions.

## Source Code for Previous Editions
- [Django 4 by Example](https://github.com/PacktPublishing/Django-4-by-Example)
- [Django 3 by Example](https://github.com/PacktPublishing/Django-3-by-Example)
- [Django 2 by Example](https://github.com/PacktPublishing/Django-2-by-Example)
- [Django by Example](https://github.com/PacktPublishing/Django-by-Example)

## Editions in Other Languages
While the 5th edition of the book is translated to other languages, you can find translations for the previous editions:
- Simplified Chinese: [Django 4实例精解](https://www.tup.tsinghua.edu.cn/booksCenter/book_09905201.html)
- Polish: [Django 4. Praktyczne tworzenie aplikacji sieciowych. Wydanie IV](https://helion.pl/ksiazki/django-4-praktyczne-tworzenie-aplikacji-sieciowych-wydanie-iv-antonio-mele,djan44.htm#format/d)
- Russian: [Django 4 в примерах](https://dmkpress.com/catalog/computer/web/978-5-93700-204-4/)
- Brazilian Portuguese: [Aprenda Django 3 com Exemplos](https://novatec.com.br/livros/aprenda-django3-com-exemplos/)
- Serbo-Croatian-Bosnian: [Django 3 kroz primere, prevod III izdanja](https://knjige.kombib.rs/django-3-kroz-primere-prevod-iii-izdanja)
- Spanish: [Django 2](https://www.amazon.es/Django-2-Antonio-Mel%C3%A9/dp/8426727484)

## Download a free PDF
If you have already purchased a print or Kindle version of this book, you can get a DRM-free PDF version at no cost. Simply click on the link to claim your free PDF: [https://packt.link/free-ebook/9781805125457](https://packt.link/free-ebook/9781805125457)

## Graphic Bundle
We also provide a PDF file that has color images of the screenshots/diagrams used in this book at [GraphicBundle](https://packt.link/gbp/9781805125457) <img alt="Coding" height="15" width="35"  src="https://media.tenor.com/ex_HDD_k5P8AAAAi/habbo-habbohotel.gif">

## Errata
- Page 39 `Post.objects.filter(id_lt=3).count()` code example should read `Post.objects.filter(id__lt=3).count()`
