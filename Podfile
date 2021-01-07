# Uncomment the next line to define a global platform for your project
# platform :ios, '9.0'

target 'SPAnyDone' do
  # Comment the next line if you don't want to use dynamic frameworks
  use_frameworks!

  # Pods for SPAnyDone
  pod 'CocoaMQTT'
  pod 'GoogleWebRTC', '~> 1.1'
  
  post_install do |installer|
    installer.pods_project.build_configurations.each do |config|
      config.build_settings["EXCLUDED_ARCHS[sdk=iphonesimulator*]"] = "arm64"
      #the following lines need to be added to podspec file because of arm64 issue
      
      #   s.pod_target_xcconfig = { 'EXCLUDED_ARCHS[sdk=iphonesimulator*]' => 'arm64'}
      #s.user_target_xcconfig = { 'EXCLUDED_ARCHS[sdk=iphonesimulator*]' => 'arm64'}
    end
  end
  
 
  


  target 'SPAnyDoneTests' do
    # Pods for testing
  end

end
