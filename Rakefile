require 'rspec/core/rake_task'
require 'rubocop/rake_task'
require 'bundler/gem_tasks'

RSpec::Core::RakeTask.new(:spec)
RuboCop::RakeTask.new

task default: :spec

desc 'Run acceptance tests (RSpec + Rubocop)'
task test: 'acceptance'

desc 'Run acceptance tests (RSpec + Rubocop)'
task :acceptance do |_t|
  Rake::Task['spec'].invoke
  Rake::Task['rubocop'].invoke
end
