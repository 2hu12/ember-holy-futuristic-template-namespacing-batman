ember-holy-futuristic-template-namespacing-batman
==============================================================================

This experimental addon allows for an additional style of invoking
components and helpers using their addons name, by using `$` syntax.

*Note:* This addon does not support using the `::` syntax that was
originally proposed in
[emberjs/rfcs#309](https://github.com/emberjs/rfcs/pull/309) (e.g.
`{{some-addon-name::component-name}}`). This was deprecated in [ember-holy-futuristic-template-namespacing-batman/233](https://github.com/rwjblue/ember-holy-futuristic-template-namespacing-batman/pull/233) in order to avoid collisions with
[emberjs/rfcs#457](https://github.com/emberjs/rfcs/pull/457).

### Requirements:

* Ember.js v3.4 or above
* Ember CLI v2.13 or above
* Node.js v8 or above

Installation
------------------------------------------------------------------------------

```
ember install ember-holy-futuristic-template-namespacing-batman
```


Usage
------------------------------------------------------------------------------

- Supports helper invocation:

```hbs
{{addon-name$helper-name}}
```

- Supports component invocation:

```hbs
{{addon-name$component-name}}
```

- Supports angle bracket invocation (when used with Ember 3.4+ or ember-angle-bracket-invocation-polyfill)

```hbs
<AddonName$ComponentName />
```

- Supports nested angle bracket invocation (when used with Ember 3.10+ or ember-angle-bracket-invocation-polyfill)

```hbs
<AddonName$SomeFolderName::ComponentName />
```

Contributing
------------------------------------------------------------------------------

### Installation

* `git clone git@github.com:rwjblue/ember-holy-futuristic-template-namespacing-batman`
* `cd ember-holy-futuristic-template-namespacing-batman`
* `npm install`

### Linting

* `npm run lint:js`
* `npm run lint:js -- --fix`

### Running tests

* `ember test` – Runs the test suite on the current Ember version
* `ember test --server` – Runs the test suite in "watch mode"
* `ember try:each` – Runs the test suite against multiple Ember versions

### Running the dummy application

* `ember serve`
* Visit the dummy application at [http://localhost:4200](http://localhost:4200).

For more information on using ember-cli, visit [https://ember-cli.com/](https://ember-cli.com/).

License
------------------------------------------------------------------------------

This project is licensed under the [MIT License](LICENSE.md).
