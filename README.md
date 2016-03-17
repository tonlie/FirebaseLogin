# firebase-login

An element that creates a login menu for firebase using Paper elements.
Includes a `<paper-menu-button>`, encapsulating a `<firebase-auth>` element and
some additional functionality regarding Firebase's own e-mail and password based
login provider.
Built to work extra great in `<paper-header-panel>`'s.

Example:
```html
<firebase-login
redirect
google
mail-pass
firebase-url='https://<YOUR-FIREBASE-APP>.firebaseio.com'>
</firebase-login>
```
@demo demo/index.html

## Dependencies

Element dependencies are managed via [Bower](http://bower.io/). You can
install that via:

    npm install -g bower

Then, go ahead and download the element's dependencies:

    bower install
