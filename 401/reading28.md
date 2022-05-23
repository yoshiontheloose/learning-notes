# API Deployment

## Reading

### Django Settings Best Practices

[Source](https://djangostars.com/blog/configuring-django-settings-best-practices/)

#### Managing Django Settings: Issues

**Different Environments**: An approach is needed to keep all Django setting configurations because each environment will have it's own specific settings.

**Sensitive Data**: Django projects hold sensitive information such as the `SECRET_KEY`, tokens, database passwords. These can't be shown in your code/project.

**Sharing settings between team members**: Developers bring human error, they may forget to add specific settings when adding an app or doing any API integration.

**Django Settings are a Python Code**: settings.py can be a problem, it has different logic than key-value pairs.

#### Setting Configuration: Different Approaches

**settings_local.py**":

Oldest method, still used today. Environment specific settings are extended in this file and ignored by VCS.

- Pros

  - Secrets not in VCS  
  
- Cons
  
  - Django environment settings can be lost.
  
  - non-obvious logic because it is Python code

  - Must have `settings_local.example` in VCS to share the configurations

**Separate settings file for each environment**:

Having a settings package with a file structure. This way you can share settings between other developers as the configurations are kept in VCS.

- Pros

  - VCS has all environments

  - developers can share the settings

- Cons

  - Tokens and secret passwords need a way to be handled

  - Hard to keep track and maintain setting inheritance

**Environment variables**:

Used to handle sensitive data.

- Pros

  - Configuration is separated from code

  - Same code for all environments

  - Cleaner and more consistent as there is no inheritance in settings

  - 12 factor structure for using environment variables

- Cons

  - Developers must handle sharing default configuration

#### 12 Factors

Created by Heroku, these are a collection of recommended points on building web apps to be deployed in the Cloud. Main rule: "store configuration in the environment" - separates config from the code.

1. Codebase

2. Dependencies

3. Config

4. Backing Services

5. Build, release, run

6. Processes

7. Port binding

8. Concurrency

9. Disposability

10. Dev/prod parity

11. Logs

12. Admin processes

</br>

### SSH Tutorial

[Source](https://www.hostinger.com/tutorials/ssh-tutorial-how-does-ssh-work)

---

## Bookmark/Skim

### White Noise

[Source](http://whitenoise.evans.io/en/stable/)

### IaaS

[Source](https://en.wikipedia.org/wiki/Infrastructure_as_a_service)

### PaaS
[Source](https://en.wikipedia.org/wiki/Platform_as_a_service)

### CORS

[Source](https://en.m.wikipedia.org/wiki/Cross-origin_resource_sharing)

---

</br>

[<<<Back](README.md)
