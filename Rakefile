require 'rubygems'
require 'rake'
require 'spec/rake/spectask'

begin
  require 'jeweler'
  Jeweler::Tasks.new do |gem|
    gem.name = "machinist_mongomapper"
    gem.summary = %Q{Machinist adapter for MongoMapper}
    gem.email = "dev@yeastymobs.com"
    gem.homepage = "http://github.com/yeastymobs/machinist_mongomapper"
    gem.authors = ["Nicolas Mérouze", "Vincent Hellot", "Mathieu Fosse"]
    
    gem.add_dependency('notahat-machinist',  '~> 1.0.3')
    gem.add_dependency('mongomapper', '~> 0.3.1')
  end
rescue LoadError
  puts "Jeweler (or a dependency) not available. Install it with: sudo gem install jeweler"
end

desc 'Default: run specs.'
task :default => :spec

desc 'Run all the specs for the machinist plugin.'
Spec::Rake::SpecTask.new do |t|
  t.spec_files = FileList['spec/**/*_spec.rb']
  t.rcov = false
end