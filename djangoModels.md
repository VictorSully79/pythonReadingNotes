# Django Models

notes taken from <https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Models>

Django uses web applications to through Python objects referred to as models.

## Designing Models

When designing models it is helpful to use a model for every object.

Models can also represent section lists.

Types of relationships 

- One -> One
- One -> Many
- many -> One

Models are located in the models.py file.

A model  can have as many fields as needed.

Below is an example of a single field:

`my_field_name = models.CharField(max_length=20, help_text='Enter field documentation')`

## Field Arguments

- help_text: Provides a text label for HTML forms (e.g. in the admin site).
- verbose_name: A human-readable name for the field used in field labels. If not specified, Django will infer the default verbose name from the field name.
- default: The default value for the field. This can be a value or a callable object, in which case the object will be called every time a new record is created.
- null: If True, Django will store blank values as NULL in the database for fields where this is appropriate (a CharField will instead store an empty string). The default is False.
- blank: If True, the field is allowed to be blank in your forms. The default is False, which means that Django's form validation will force you to enter a value. This is often used with
- null=True , because if you're going to allow blank values, you also want the database to be able to represent them appropriately.
- choices: A group of choices for this field. If this is provided, the default corresponding form widget will be a select box with these choices instead of the standard text field.
- primary_key: If True, sets the current field as the primary key for the model (A primary key is a special database column designated to uniquely identify all the different table records). If no field is specified as the primary key then Django will automatically add a field for this purpose.

