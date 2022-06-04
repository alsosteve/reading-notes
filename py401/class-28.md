# [Reading-Notes](https://alsosteve.github.io/reading-notes/)
Code Fellows Python 401

# Read: 28 - Django CRUD and Forms

## [Django Forms](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Forms)

### HTML Form 
- is a group of one or more fields/widgets on a web page
- used to collect info from users
- flexible
#### example:
![html](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Forms/form_example_name_field.png)

``` html
<form action="/team_name_url/" method="post">
    <label for="team_name">Enter name: </label>
    <input id="team_name" type="text" name="name_field" value="Default name for team.">
    <input type="submit" value="OK">
</form>
```
### Form Handling Process
![ex of form handling process](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Forms/form_handling_-_standard.png)

### Form Class
- specifies fields in form
- provides methods for rendering itself
- predefined formats (tables, lists, etc.)

### Declaring a Form
- similar to declaring a Model

``` python
from django import forms

class RenewBookForm(forms.Form):
    renewal_date = forms.DateField(help_text="Enter a date between now and 4 weeks (default 3).")
```

### Form fields
> The arguments that are common to most fields are listed below (these have sensible default values):

- required
- label
- label_suffix
- initial
- widget
- help_text
- error_message
- validators
- localize
- disable

### Validation
how to validate your data
- to validate a single field use `clean_<fieldname>()` method

## Bookmark and Review
- [Django Templates](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Home_page)
- [Django Views](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Generic_views)