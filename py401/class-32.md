# [Reading-Notes](https://alsosteve.github.io/reading-notes/)
Code Fellows Python 401

# Read: 32 - Permissions & Postgresql

## [DRF Permissions](https://www.django-rest-framework.org/api-guide/permissions/)
> Authentication or identification by itself is not usually sufficient to gain access to information or code. For that, the entity requesting access must have authorization. — Apple Developer Documentation

- Permission checks are always run at the very start of the view
- use the authentication information
- used to grant or deny access for different classes
- defined as a list of permission classes

### Object level permissions
- used to determine if a user should be allowed to act on a particular object
- run by REST framework's generic views
-will not automatically apply object level permissions

## Bookmark and Review
- [Classy Django REST](http://www.cdrf.co/)
- [DRF Generic Views](https://www.django-rest-framework.org/api-guide/generic-views/)