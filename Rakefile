# -*- coding: utf-8 -*-
$:.unshift("/Library/RubyMotion/lib")
require 'motion/project/template/ios'

begin
  require 'bundler'
  Bundler.require
rescue LoadError
end

Motion::Project::App.setup do |app|
  app.name = 'btle'
  # Use `rake config' to see complete project settings.
  app.vendor_project("vendor/HXMBLEConnectionManager",
    :products => ["libhxm2sdk.a"],
    :headers_dir => "HXMBLEConnectionManager.h", "PhysiologicalData.h" )
  app.frameworks << 'Foundation'
  app.frameworks << 'CoreBluetooth'
  app.frameworks << 'UIKit'
  app.frameworks << 'CoreGraphics'

end
