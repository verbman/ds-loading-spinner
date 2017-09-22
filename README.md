# Loading spinner

## About the component

An accessible loading/progress spinner shown when actions take a period of time. Optionally can show a message/percentage that counts up.


## Demo
- [Loading spinner prototype](https://govuk-loader-prototype.herokuapp.com/components/loader)
- [Loading spinner with generic message](https://govuk-loader-prototype.herokuapp.com/components/loader-message)
- [Loading spinner with updating message](https://govuk-loader-prototype.herokuapp.com/components/loader-progress)
- [Loading spinner with different backgrounds](https://govuk-loader-prototype.herokuapp.com/components/loader-inverted)

## Dependencies
Accessible-loading-spinner has [govuk_elements](https://github.com/alphagov/govuk_elements) as a dependency.

## Usage
Copy the [app/assets/javascript/loader.js](https://github.com/alex-ju/accessible-loading-spinner/blob/master/app/assets/javascripts/loader.js) file to your JavaScript folder and import it into the browser:

`<script type="text/javascript" src="assets/js/accessible-autocomplete.min.js"></script>`

Copy the [app/assets/sass/patterns/_loader.scss](https://github.com/alex-ju/accessible-loading-spinner/blob/master/app/assets/sass/patterns/_loader.scss) to your Sass folder and import it:

`@import "loader";`

Initialize the component by specifying the container (e.g. ``govuk-box``) that will contain the loading spinner.

### Basic loading spinner
```
var loadingSpinner = new GOVUK.Loader()
loadingSpinner.init({
  container: 'govuk-box'
})
```

### Loading spinner with generic message
```
var loadingSpinner = new GOVUK.Loader()
loadingSpinner.init({
  container: 'govuk-box',
  label: true
})
```

### Loading spinner with updating message
```
var loadingSpinner = new GOVUK.Loader()
loadingSpinner.init({
  container: 'govuk-box',
  label: true
})
```
For updating the label call
```
loadingSpinner.updateMessage('10%')
```

## Options
You can configure the loading spinner by passing optional arguments when initializing the component as follows:
```
var loadingSpinner = new GOVUK.Loader()
loadingSpinner.init({
  container: 'govuk-box'
  labelText: 'Loading...',
  label: true,
  color: '#000'
})
```
