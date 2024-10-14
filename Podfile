# Uncomment the next line to define a global platform for your project
# platform :ios, '11.0'

target 'private pe' do
  # Comment the next line if you don't want to use dynamic frameworks
  use_frameworks!

  # Pods for private pe
  target 'private peTests' do
    inherit! :search_paths
  end

  target 'private peUITests' do
  end
  
  pod 'GoogleSignIn', '~> 5.0'
  pod 'IQKeyboardManagerSwift'
  pod 'NVActivityIndicatorView'
  pod 'SwiftMessages'
  pod 'Kingfisher'
  pod 'MBProgressHUD'
  pod 'SwiftyJSON'
  pod 'TYPagerController' , '~> 2.0.1'
  pod 'SDWebImage', '~> 5.0'
  pod 'lottie-ios'
  pod 'SkeletonView'
  pod 'TXLiteAVSDK_TRTC', :podspec => 'https://liteav.sdk.qcloud.com/pod/liteavsdkspec/TXLiteAVSDK_TRTC.podspec'
  pod 'Firebase/Firestore'
  pod 'TXIMSDK_Plus_iOS'
  pod 'Firebase/Database'
  pod 'SQLite.swift', '~> 0.12.2'
  pod 'SVGAPlayer'
  pod 'BDAlphaPlayer'
  pod 'Alamofire'
  pod 'IJKMediaFramework'
  pod 'Firebase/Crashlytics'

  post_install do |installer_representation|
    installer_representation.pods_project.targets.each do |target|
      target.build_configurations.each do |config|
        config.build_settings['ONLY_ACTIVE_ARCH'] = 'NO'
        config.build_settings['BUILD_LIBRARY_FOR_DISTRIBUTION'] = 'YES'
        config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = "13.0"
        config.build_settings['EXCLUDED_ARCHS[sdk=iphonesimulator*]'] = 'arm64'
      end
    end
  end
end
