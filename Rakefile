require 'rubygems/package_task'

spec = Gem::Specification.load(Dir['*.gemspec'].first)
gem = Gem::PackageTask.new(spec)
gem.define()

Dir.glob('lib/tasks/*.rake').each { |r| import r }

#gem push pkg/heroku-mongo-backup-version.gem