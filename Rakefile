require 'rubygems'
require 'rack/test'
require 'rake/clean'
require 'rspec/core'
require 'rspec/core/rake_task'

RSpec::Core::RakeTask.new(:spec) do |spec|
  spec.pattern = 'spec/**/*_spec.rb'
end

RSpec::Core::RakeTask.new(:cov) do |spec|
  spec.pattern = 'spec/**/*_spec.rb'
  spec.rcov = true
end

task :default => :spec

# output directory - removed with "rake clobber" (needs a "require 'rake/clean'" above)
CLOBBER.include("coverage")
