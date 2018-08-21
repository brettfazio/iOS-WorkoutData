platform :ios, '11.0'
inhibit_all_warnings!

def di_pods
  pod 'Swinject', '~> 2.4.1'
  pod 'SwinjectAutoregistration', '~> 2.1.1'
end

def helper_pods
  pod 'Alamofire', '~> 4.7'
  pod 'PromiseKit', '~> 6.3.4'
  pod 'RealmSwift', '~> 3.7'
  pod 'Sourcery', '~> 0.13'
  pod 'SwiftLint', '~> 0.27'
end

def test_pods
  pod 'Nimble-Snapshots', '~> 6.7.1'
  pod 'Nimble', '~> 7.1.3'
  pod 'Quick', '~> 1.3.1'
end

def ui_pods
  pod 'Reveal-SDK', :configurations => ['Debug']
  pod 'SnapKit', '~> 4.0.0'
end

target 'WorkoutData' do
  use_frameworks!
  di_pods
  helper_pods
  ui_pods

  target 'WorkoutDataTests' do
    inherit! :search_paths
    test_pods
  end
end