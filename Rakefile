require 'rubygems/package_task'
gemspec = Gem::Specification.load(Dir['*.gemspec'].first)
Gem::PackageTask.new(gemspec).define

require 'rspec/core/rake_task'
RSpec::Core::RakeTask.new(:spec) do |spec|
  spec.pattern = 'spec/**/*_spec.rb'
end
task :default => :spec

