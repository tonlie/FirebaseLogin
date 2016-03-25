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

## Usage
Add the element to your app using the `<firebase-login>` tag. This will create a
button that implements the login functionality.

### Properties
For the element to work, the following properties must be set:
* `firebaseUrl`
* at least one of the providers (e.g. `facebook`, `google`, ...)

| Name | Type | Default | Description |
| --- | --- | --- | --- |
| `autoLogin` | Boolean | false | Activate automatic login, see firebase-element |
| `facebook` | Boolean | false – notifies | facebook enables facebook authentication provider |
| `firebaseRef` | Object | readOnly | Firebase reference object |
| `firebaseUrl` | string || firebaseUrl contains the URL to the firebase instance |
| `github` | Boolean | false – notifies | github enables github authentication provider |
| `google` | Boolean | false – notifies | google enables google authentication provider |
| `mailPass` | Boolean | false – notifies | mailPass enables firebases own e-mail & password provider |
| `maxWidth` | String | 640px – notifies | Max-width for media query for the drawer-panel. To deactivate the drawer-panel, set this to 0px. |
| `redirect` | Boolean | false | Should login try redirect, see firebase-element |
| `statusKnown` | Boolean | false – readOnly | statusKnown determines, whether there is a user logged in |
| `twitter` | Boolean | false – notifies | twitter enables twitter authentication provider |

### Styling
The element can be styled like most other elements using css.

The following custom properties are also available for styling (see: https://www.polymer-project.org/1.0/docs/devguide/styling.html#xscope-styling-details):

| Custom property | Description | Default |
| --- | --- | --- |
| `--firebase-login-button-background` | Background color of the paper-menu-button | `--accent-color` |
| `--firebase-login-button-text` | Text color of the paper-menu-button | `--text-primary-color` |
| `--firebase-login-menu-item-hover-background` | Background color of the paper-menu-button (e.g. 'Login with Google') | `--accent-color` |
| `--firebase-login-menu-item-hover-text` | Text color of the paper-menu-items (e.g. 'Login with Google') | `--text-primary-color` |
| `--firebase-login-dialog-tabs-background-color` | Background color of the paper-tabs in e-mail and password provider dialog | `--accent-color` |
| `--firebase-login-dialog-tabs-text-color` | Text color of the paper-tabs in e-mail and password provider dialog | `--text-primary-color` |
| `--firebase-login-dialog-button-text-color` | Text color of the paper-buttons in e-mail and password provider dialog | `--accent-color` |
| `--firebase-login-toast-success-background` | Background color of the successfull toast messages | `#4CAF50` |
| `--firebase-login-toast-error-background` | Background color of the unsuccessfull toast messages | `#FF5252` |

### Dependencies

Element dependencies are managed via [Bower](http://bower.io/). You can
install that via:

    npm install -g bower

Then, go ahead and download the element's dependencies:

    bower install
