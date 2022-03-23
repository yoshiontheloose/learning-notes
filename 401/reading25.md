# Django REST Framework & Docker

## Reading

### Beginner’s Guide to Docker

[Source](https://wsvincent.com/beginners-guide-to-docker/)

Docker - "A way to isolate and run entire applications." Docker is a sharable way to run Linux containers, multiple people can work on the same setup. The containers are an alternative to using virtual machines.

The amount of size and speed are the downsides to using a virtual machine. Also, they can only isolate Python packages.

An analogy from the article: Virtual machines are like homes, while Docker containers are like apartments.

**Images**- "A snapshot in time of what a project contains"

**Containers**- "A running instance of the image"

Dockerfiles are read from top to bottom.

`FROM` command **MUST** be the first instruction.

**Image Layering**- Each image has image layers, at least one or more, and the layers are unchanged/immutable. This helps with performance and consistency while more than one developer build the same image.

Order matters, code that will change the least at the top and code that will change the most on the bottom.

`docker-compose.yml` - "controls how to run the container"

### Django for APIs - Library Website

[Source](https://djangoforapis.com/library-website-and-api/)

Django REST framework- creates web APIs with the Django web framework. Django is needed to use Django REST.

This article explains setting up a Django project in a convenient and straightforward way.

---

## Bookmark/Skim

### Beginner’s Guide to Django REST Framework

[Source](https://wsvincent.com/official-django-rest-framework-tutorial-beginners-guide)

---

</br>

[<<<Back](README.md)
