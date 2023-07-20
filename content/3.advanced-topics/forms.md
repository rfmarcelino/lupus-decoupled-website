# Forms

Forms can be implemented using the [Webform module](https://www.drupal.org/project/webform), so that you can render webforms into custom elements.

Note: Currently not implemented, but planned for the future.

## Use webforms

Webforms are created in the Drupal UI using the form builder.

Create a new form:

**Administration** > **Webforms** > **Add webform**

Here you can add fields to the form, and configure the form settings.

## Render webforms

Webforms are rendered by Drupal-CE into custom elements, which can be used in your frontend.

Example of a webform rendered into a custom element:

```json
"element": "webform",
"title": "Contact",
"webformCE": [
  {
    "element": "webform-ce",
    "content": "<form>...</form"
  }
]
```