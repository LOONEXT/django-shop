# django-SHOP

[![Build Status](https://travis-ci.org/awesto/django-shop.svg?branch=master)](https://travis-ci.org/awesto/django-shop.svg?branch=master)
[![PyPI version](https://img.shields.io/pypi/v/django-shop.svg)](https://https://pypi.python.org/pypi/django-shop)
[![Join the chat at https://gitter.im/awesto/django-shop](https://badges.gitter.im/awesto/django-shop.svg)](https://gitter.im/awesto/django-shop?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
[![Twitter Follow](https://img.shields.io/twitter/follow/shields_io.svg?style=social&label=django-SHOP&maxAge=2592000)](https://twitter.com/djangoshop)

Version 0.10 of **django-SHOP** is heading towards API stability. Before upgrading to this version
please read carfully the Changelog, as the API has been simplified and now is much more generic than
in version 0.9.

Please get in touch with us on Gitter, if you have problems to upgrade your 0.9 projects. This will
help us to adopt the migration path.


## Running the demo projects

To get a first impression on **django-SHOP**, try out one of the six fully working demo projects.


### Run the demo in a local virtualenv

Following the [introduction instructions](http://django-shop.readthedocs.io/en/latest/tutorial/intro.html)
should create a running shop in minutes, prefilled with a dozen of products. You can even pay by credit
card, if you apply for your own testing account at Stripe.


### Run the demo using Docker

A faster alternative to run one of the demos of **django-SHOP**, is to use a prepared Docker
container available on the [Docker Hub](https://hub.docker.com/r/awesto/demo-shop/).
If you have a running docker-machine, download and start the demo using:

```
docker run --name demo-shop-i18n_polymorphic --env DJANGO_SHOP_TUTORIAL=i18n_polymorphic -p 9001:9001 awesto/demo-shop:latest
```

Then point a browser on the IP address of your docker machine onto port 9001. If unsure invoke
``docker-machine ip``. This for instance could be http://192.168.99.100:9001/ .
To access the backend, sign in with username *admin* and password *secret*. The first invocation
may take a few minutes, since additional assets have to be downloaded and the supplied images have
to be thumbnailed.


## Current Status of Django-SHOP

This version of django-SHOP is currently used to implement real e-commerce sites. If you want
to get involved in the development, please have a look at our documentation in ``docs/contributing.rst``.


**Django-SHOP** aims to be a the easy, fun and fast shop counterpart to **django-CMS**.

Specifically, we aim at providing a clean, modular and Pythonic/Djangonic implementation of an
e-commerce framework, that a moderately experienced Django developer should be able to pick up
and run easily.

Whenever possible, extra features shall be added to third party libraries. This implies that
**django-SHOP** aims to provide an API, which allows merchants to add every feature they desire.
