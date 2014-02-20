*This repository is a mirror of the [component](http://component.io) module [yields/visibility](http://github.com/yields/visibility). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/yields-visibility`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# visibility

  Sane page visibility API

## Installation

    $ component install yields/visibility

## API

### visibility([fn])

```javascript
visibility(function (e, state) {
  if ('visible' == state) dostuff();
});
```

### visible(fn)

Execute the given `fn` when the page is visible.
```javascript
visibility()
  .visible(function (e) {});
```

### hidden(fn)

Execute the given `fn` when the page is hidden.
```javascript
visibility()
  .hidden(function (e) {});
```

### prerender(fn)

Execute the given `fn` on prerender.

```javascript
visibility()
  .prerender(function () {});
```

## todo

  * add tests.
  * test in all browsers, currently tested only in Chrome.


## License

  MIT
