[Home](../README.md)

## Class 09

### HTML Forms

- Forms are important in web development because a form is one of the most fundamental ways that sites can interact with users and receive information from them.
- Forms generally either send received data to a web server to be processed, or  use received data to update the sites content or styling in some way.
- Some good things to keep in mind when designing forms are keeping things simple, designing a mockup, and ensuring the form is usable and self-explanatory.
- Here are some common form elements:
  - `<form>` - this is the main form element, and contains the other elements that comprise the content of your form.
    - the `action` attribute defines where a forms data should go when submitted (URL).
    - the `method` attribute says which HTTP method to send the data in (usually `get` or `post`).
  - `<label>` - this defines the label that will sit next to an adjacent input field.
  - `<input>` - this is a single line input field that can be given attributes to provide integrated form validation, sush as taking only text, numbers, emails, etc.
  - `<textarea>` - this is a multiline input field for things such as email correspondence or other messages and long-form responses.
  - `<button>` - this element is fairly self-explanatory, and allows a user to let the site know when they're done with the form and submit

### JS Events

- Events are essentially anything that happens or changes on a web page. User actions, changes of state for elements, etc.
- The `addEventListener` method tells an object or element to listen for an event and perform an action when it hears it. The two arguments are the event to listen for and the function to execute.
- The event object is an argument that is automatically passed to an event handler. Its target propoerty is useful because it allows us to write event functions that occur relative to the element(s) that are targeted. This allows us to reuse that function for potentially many different elements.
- Some event objects have special properties, such as the `KeyboardEvent`, which has a built in `key` property that returns which key was pressed
- Event bubbling and capturing refer to the order in which events are fired on the hierarchy of elements
  - bubbling refers to an event firing first on its innermost element, and then on every supsequent parent
  - capturing is the opposite, and fires the event on the outermost parent (`<html>`) and then proceeds to fire on each subsequent child until the target element
