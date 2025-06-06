(styleguide)=

# UI Styleguide

Developers working on the Wagtail UI or creating new UI components may wish to test their work against our Styleguide, which is provided as the contrib module "wagtailstyleguide".

To install the styleguide module on your site, add it to the list of `INSTALLED_APPS` in your settings:

```python
INSTALLED_APPS = (
    # ...
    'wagtail.contrib.styleguide',
    # ...
)
```

This will add a 'Styleguide' item to the Settings menu in the admin.

At present the styleguide is static: new UI components must be added to it manually, and there are no specific hooks into it for other modules to use. It will include the output of the [](insert_editor_js) hook for any custom edit forms JavaScript that may be used.

We hope to support specific styleguide hooks in the future.

The styleguide doesn't currently provide examples of all the core interface components; notably the Page, Document, Image and Snippet chooser interfaces are not currently represented.
