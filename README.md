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
