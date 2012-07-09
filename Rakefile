# encoding: utf-8

require 'rubygems'
require 'bundler'
begin
  Bundler.setup(:default, :development)
rescue Bundler::BundlerError => e
  $stderr.puts e.message
  $stderr.puts "Run `bundle install` to install missing gems"
  exit e.status_code
end
require 'rake'

require 'jeweler'
Jeweler::Tasks.new do |gem|
  # gem is a Gem::Specification... see http://docs.rubygems.org/read/chapter/20 for more options
  gem.name = "dark-capistrano-recipes"
  gem.homepage = "http://github.com/darkside/capistrano-recipes"
  gem.license = "MIT"
  gem.summary =%q{Capistrano recipes}
  gem.description = %q{Extend the Capistrano gem with these useful recipes}
  gem.email = "leonardobighetti@gmail.com"
  gem.authors = ["Phil Misiowiec", "Leonardo Bighetti", "Rogerio Augusto"]
  # dependencies defined in Gemfile

end
Jeweler::RubygemsDotOrgTasks.new

require 'rdoc/task'
Rake::RDocTask.new do |rdoc|
  version = File.exist?('VERSION') ? File.read('VERSION') : ""

  rdoc.rdoc_dir = 'rdoc'
  rdoc.title = "dark-capistrano-recipes #{version}"
  rdoc.rdoc_files.include('README*')
  rdoc.rdoc_files.include('lib/**/*.rb')
end

