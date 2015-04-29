### Read Countries in YAML and JSON

Read and parse Countries Data YAML and JSON files in Ruby.

##### YAML:
```ruby
yaml_file = YAML.load_file('countries.yml')

yaml_file.each do |country|
  name = country["name"]
  code = country["code"]
  
  puts "#{name} code is: '#{code}'" #=> Uruguay code is: 'UY'
end
```
##### JSON:
```ruby
json_file = File.read('countries-object-array.json.json')
all_countries = JSON.parse(json_file)

all_countries.each do |country|
  name = country["name"]
  code = country["code"]
  puts "#{name} code is => '#{code}'" #=> Finland code is: 'FI'
end
```


### Credits:
A list of countries : https://gist.github.com/Keeguon/2310008
