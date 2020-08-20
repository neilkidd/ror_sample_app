![Test && Deploy](https://github.com/neilkidd/ror_sample_app/workflows/Ruby%20Test%20and%20Deploy/badge.svg)

# Ruby on Rails Tutorial Sample application

This is the sample application for [*Ruby on Rails Tutorial:Learn Web Development with Rails*](https://www.railstutorial.org/) (6th Edition) by [Michael Hartl](https://www.michaelhartl.com/).

## License

All source code in the [Ruby on Rails Tutorial](https://www.railstutorial.org/) is available jointly under the MIT License and the Beerware License. See [LICENSE.md](LICENSE.md) for details.

## Getting started

To get started with the app, clone the repo and then install the needed gems:  
```$ bundle install --without production```

Next, migrate the database:  
```$ rails db:migrate```

Finally, run the test suite to verify that everything is working correctly:  
```$ rails test```

If the test suite passes, you'll be ready to run the app in a local server:  
```$ rails server```

For more information, see the [*Ruby on Rails Tutorial* book](https://www.railstutorial.org/book).

## Notes

### Adding Guard

- `bundle exec guard init`
- Overwrite the generated [Guardfile](Guardfile) with content from [Github](https://github.com/mhartl/sample_app_6th_ed/blob/master/Guardfile).
- `bundle exec guard` to run tests on save.

### Configuring VS code

- See [The three extensions you need for Rails development in VS Code](https://dev.to/vvo/the-three-extensions-you-need-for-rails-in-vs-code-5h7j)

Add gems to the project. I pinned the versions then ran `bundle install`.
- `bundle add solargraph --group "development"`
- `bundle add rubocop --group "development"`
