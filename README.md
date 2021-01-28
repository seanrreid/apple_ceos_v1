### Apple CEOs v1

* Build an Express app that shows a list of Apple CEOs
  * `npm init -y`
  * Update any references to `index.js` to `app.js`
  * Create `script` entries for `npm start` and `npm run dev`
* It will follow the MVC Design Pattern

#### Model

* Download the `db.js` file from this repository.
  * Add this file to the root directory of the application

#### Views

* Create the following templates
  * `template.html`
  * `partials/home.html`
  * `partials/ceo-list.html`
  * `partials/ceo-details.html`
* The Root Route will return a homepage
  * This will load the `home` partial
  * Include a link to `/ceos` from this page
* The `/ceos` route will return a list of Apple CEOs
  * Load this data from the `db.js` file.
  * Render the list via the `ceo-list` partial
* The `/ceos/:slug` route will return details of a specific CEO
  * Load this data based on the `slug` entry in the `db.js` file
  * Render this page via the `ceo-details` partial

#### Controllers

* We will use the following routes
  * Root Route, `/`
  * CEOs Route, `/ceos`
  * Individual CEO route, `/ceos/:slug`