# Installing Pods
This is a simple project to install pods inside a XCode project

To create a podfile inside your project, you need to instal the `CocoaPods` inside your terminal.

To install, you will use the following command: `sudo gem install cocoapods`.

After installing CocoaPods, access your project folder inside your terminal and type the command: `pod init`.

This command will create a new file inside your project named `Podfile`.

## Structure of Podfile
The Podfile created inside your project will have the following structure:

```
# Uncomment the next line to define a global platform for your project
# platform :ios, '9.0'

target 'InstallingPods' do
  # Comment the next line if you're not using Swift and don't want to use dynamic frameworks
  use_frameworks!

  # Pods for InstallingPods
  
  target 'InstallingPodsTests' do
    inherit! :search_paths
    # Pods for testing
  end

  target 'InstallingPodsUITests' do
    inherit! :search_paths
    # Pods for testing
  end

end

```

To add a new pod inside your project, you just need to add the line: `pod 'your-pod-name-here'` below the `Pods for InstallingPods` line.

After add your pod, you comeback to the terminal and type the command: `pod install`.

This will add the pod inside your project and create a new file called that have a `workspace` name inside the file extension.

If you want to use the installed pod inside your project, you will always open your project using this workspace file.
