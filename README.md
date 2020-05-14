# Boiled Page error page singleton

Error page SCSS singleton for Boiled Page frontend framework. It is intended to create full height error pages.

## Install

Place `_error-page.scss` file to `/assets/css/singletons` directory, and add its path to singleton block in `assets/css/app.scss` file.

## Usage

### Classes

Class name | Description | Example
---------- | ----------- | -------
`error-page` | Applies page error. | `<main class="error-page"></main>`
`error-page--has-navbar` | Substracts the value of `$navbar-height` (or `$medium-navbar-height` on medium or smaller breakpoints) SCSS variables from viewport's height. By default, these variables are declared in navbar singleton. | `<main class="error-page error-page--has-navbar"></main>`

### Examples

#### Example 1

The following example shows a 404 error page. Do not forget to add `main` id when skiplink is used.

```html
<main class="error-page">
  <div class="container container--half">
    <h1>404 - Page not found</h1>
    <p>We are sorry, the page you requested cannot be found. The page you're looking for is no longer available or The URL may be misspelled.</p>
  </div>
</main>
```
