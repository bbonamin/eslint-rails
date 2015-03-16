# eslint-rails

Run [ESLint][] against your Rails repo.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'eslint-rails'
```

## Usage

### CLI

![rake-eslint-rails-run][]

```sh
rake eslint:run
```

This will analyze `application.js`. Optionally, you can supply a filename to the
task. To analyze `woop.js`, you would run

```sh
rake eslint:run[woop]
```

### Web interface

On non-production environments, visit these URLs on your application:

Path                         | Description
---------------------------- | -------------------------------------------------
`/eslint`                    | Optionally supply a filename parameter to analyze a file other than `application.js`, e.g.  `/eslint?filename=foo` to analyze foo.js.
`/eslint/source/application` | Optionally replace `application` with the name of another JavaScript file, e.g.  `eslint/source/button_stuff` will show you `button_source.js`.

![eslint-rails-web](https://cloud.githubusercontent.com/assets/324632/6671966/33d8cc86-cbc6-11e4-904d-3379907c429d.png)

![eslint-rails-web-source](https://cloud.githubusercontent.com/assets/324632/6671965/33d6819c-cbc6-11e4-9a64-30be84f20b96.png)

# Authors

- Jon Kessler &lt;[jon.kessler@appfolio.com][]&gt;
- Justin Force &lt;[justin.force@appfolio.com][]&gt;

# License

[MIT License][].

[ESLint]: http://eslint.org/
[justin.force@appfolio.com]: mailto:justin.force@appfolio.com
[jon.kessler@appfolio.com]: mailto:jon.kessler@appfolio.com
[MIT License]: http://www.opensource.org/licenses/MIT)

[rake-eslint-rails-run]: https://cloud.githubusercontent.com/assets/324632/6671891/b5b92760-cbc5-11e4-8a3c-12c19ccfbb4d.png
[eslint-rails-web-source]: https://cloud.githubusercontent.com/assets/324632/6671965/33d6819c-cbc6-11e4-9a64-30be84f20b96.png
[eslint-rails-web]: https://cloud.githubusercontent.com/assets/324632/6671966/33d8cc86-cbc6-11e4-904d-3379907c429d.png