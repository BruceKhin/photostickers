source 'https://github.com/jjochen/podspecs.git'
source 'https://github.com/CocoaPods/Specs.git'

platform :ios, '10.0'
use_frameworks!
inhibit_all_warnings!


target 'PhotoStickers' do
    pod 'RxSwift'
    pod 'RxCocoa'
    pod 'RxDataSources'
    pod 'RealmSwift'
    pod 'RxRealm'
    pod 'Log'
    #pod 'RxSwiftExt'
    #pod 'RxCoreData'
    #pod 'RxViewModel'
    #pod 'RxOptional'
    #pod 'SnapKit'
    #pod 'Toaster'

    target 'PhotoStickersTests' do
        inherit! :search_paths
        pod 'RxTest'
        #pod 'RxBlocking'
        #pod 'Quick'
        #pod 'Nimble'
        #pod 'RxNimble'
    end
end

target 'MessageExtension' do
    pod 'RxSwift'
    pod 'RxCocoa'
    pod 'RxDataSources'
    pod 'RealmSwift'
    pod 'RxRealm'
    pod 'Log'
end

post_install do |installer|
    installer.pods_project.targets.each do |target|
        target.build_configurations.each do |config|
            config.build_settings['SWIFT_VERSION'] = '3.0'
        end
    end
end

