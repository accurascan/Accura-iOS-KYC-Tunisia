# Uncomment the next line to define a global platform for your project
platform :ios, '12.0'

target 'AccuraSDK' do
  # Comment the next line if you're not using Swift and don't want to use dynamic frameworks
  use_frameworks!
  
pod 'TesseractOCRSDKiOS'
pod 'GoogleMLKit'
pod 'AccuraLiveness_FM', '4.3.1'

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '11.0'
    end
  end
end
end
