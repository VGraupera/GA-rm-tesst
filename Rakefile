# -*- coding: utf-8 -*-
$:.unshift("/Library/RubyMotion/lib")
require 'motion/project/template/ios'

begin
  require 'bundler'
  Bundler.require
rescue LoadError
end

Motion::Project::App.setup do |app|
  # Use `rake config' to see complete project settings.
  app.name = 'GA-test'

    app.frameworks += ['CoreData', 'SystemConfiguration']
     app.libs << "/usr/lib/libz.dylib"

  app.vendor_project('vendor/GoogleAnalytics', :static,  :products => ['libGoogleAnalyticsServices.a'])
                     #, :cflags =>'"-force_load\ vendor/GoogleAnalytics/libGoogleAnalyticsServices.a"' )
  #app.vendor_project('vendor/GoogleAnalytics', :static, :cflags =>'"-force_load\ GoogleAnalyticsServices"')
end
