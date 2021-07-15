### Rspec
- rails g rspec:install
```
--color
--format documentation
```

- config/application.rb
```
config.generators do |g|
  g.test_framework :rspec,
                   fixtures: false,
                   view_specs: false,
                   helper_specs: false,
                   routing_specs: false,
                   controller_specs: false
end
```

### Factory Bot
- rspec helper
```
config.include FactoryBot::Syntax::Methods
```

- config/application.rb
  - can be added to the same generator config used for rspec
```
config.generators do |g|
  g.factory_bot suffix: 'factory'
end
```
