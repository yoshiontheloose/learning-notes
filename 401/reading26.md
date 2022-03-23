# Permissions & Postgresql

## Reading

### DRF Permissions

[Source](https://www.django-rest-framework.org/api-guide/permissions/)

**Permissions** - used for determining access requests. Checks are run at the start of the view. Properties and their authentication info used: `request.user` and `request.auth`

`IsAuthenticated` REST framework class allows access to authenticated users and denies unauthenticated users.

`IsAuthenticatedOrReadOnly` REST framework class allows full access to authenticated users and read-only access to unauthenticated users.

`exceptions.PermissionDenied` or `exceptions.NotAuthenticated` indicate a failed permission list check on the main body of the view and it will not run.

**Object level permissions** - typically used with model instances to determine a user action

`.get_object()` runs object level permissions with rfw's generic views

`exceptions.PermissionDenied` indicates user cannot take action on the given object

`.check_object_permissions(request, obj)` used when enforcing object level permissions on views you wrote or if you override the `get_object` method on a generic view.

- Raises `PermissionDenied` or `NotAuthenticated` exceptions

**Setting Permission Policy**:

Globally set default permission policy

``` markdown
REST_FRAMEWORK = {
    'DEFAULT_PERMISSION_CLASSES': [
        'rest_framework.permissions.IsAuthenticated',
    ]
}
```

Allows unrestricted access

```markdown
'DEFAULT_PERMISSION_CLASSES': [
   'rest_framework.permissions.AllowAny',
]
```

---

## Bookmark/Skim

### Classy Django REST

[Source](http://www.cdrf.co/)

### DRF Generic Views

[Source](https://www.django-rest-framework.org/api-guide/generic-views/)

---

</br>

[<<<Back](README.md)
