require 'rubygems/package_task'
require 'rake/testtask'

spec = Gem::Specification.new do |s|
  s.name         = 'solarb'
  s.version      = '0.0.1'
  s.date         = '2018-01-21'
  s.summary      = "Photovoltaik System Overview"
  s.description  = "Programatic access to the SMA Solar Technology AG Sunny Portal"
  s.authors      = ["Daniel Bovensiepen"]
  s.email        = 'daniel@bovensiepen.net'
  s.files        = Dir.glob("{bin,lib}/**/*") + %w(LICENSE README.md)
  s.executables  = ['solarb']
  s.homepage     = 'https://github.com/bovi/solarb'
  s.license      = 'MIT'
end

Gem::PackageTask.new(spec) do |pkg|
  pkg.need_zip = true
  pkg.need_tar = true
end

task :clean => [:clobber_package]
