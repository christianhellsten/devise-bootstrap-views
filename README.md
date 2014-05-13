# Devise Bootstrap Views

Here are some of the highlights:

* Bootstrapified View
* Responsive
* I18n Support

This gem copies most of its code from [devise-i18n-views](https://github.com/mcasimir/devise-i18n-views) gem.

## Screenshot
![Screenshot](https://github.com/hisea/devise-bootstrap-views/raw/master/screenshot.png)

## Installation

Add this line to your application's Gemfile:

    gem 'devise-bootstrap-views'

And then execute:

    $ bundle

Add some minor css fix to your rails asset pipeline manifest

    *= require devise_bootstrap_views

Then you need to install the required translations in your `config/locales`. You can do this either manually (downloading them from [devise-i18n-views/locales](https://github.com/mcasimir/devise-i18n-views/tree/master/locales)) or through the apposite generator `devise:views:locale`, eg.

``` sh
rails g devise:views:locale it
```

will generate `config/locales/devise.views.it.yml`.

## Customizing Views

The `devise:views:bootstrap_templates` generator will copy all views to your application, so you can modify the files as you wish:

``` sh
rails g devise:views:i18n_templates
```

## Contributing

1. Fork it ( https://github.com/hisea/devise-bootstrap-views/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
