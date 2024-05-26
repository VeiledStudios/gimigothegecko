platform :ios, '12.0'

target 'GimigoTheGecko' do
  use_frameworks!
  
  pod 'Alamofire', '~> 5.4'

  target 'GimigoTheGeckoTests' do
    inherit! :search_paths
  end

  target 'GimigoTheGeckoUITests' do
  end
end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '12.0'
    end
  end
end

