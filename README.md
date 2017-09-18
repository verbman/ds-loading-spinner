# Loading spinner

## About the component

An accessible loading/progress spinner shown when actions take a period of time. Optionally can show a message/percentage that counts up.


## Demo

- [Loading spinner prototype](https://govuk-loader-prototype.herokuapp.com/components/loader)
- [Loading spinner with generic message](https://govuk-loader-prototype.herokuapp.com/components/loader-message)
- [Loading spinner with updating message](https://govuk-loader-prototype.herokuapp.com/components/loader-progress)
- [Loading spinner with different backgrounds](https://govuk-loader-prototype.herokuapp.com/components/loader-inverted)


## Usage
Initialize the component by specifying the container (e.g. ``govuk-box``) that will contain the loading spinner.
```
var loader = new GOVUK.Loader()
loader.init({
  container: 'govuk-box'
})
```

## Options
There are a couple of options that you can pass as arguments when initializing the component
```
var charCount = new GOVUK.CharCount()
charCount.init({
  selector: '.js-word-count',
  labelText: 'Loading...',
  label: true,
  progress: 50,
  color: '#000'
})
```
