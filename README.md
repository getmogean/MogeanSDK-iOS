# **MogeanSDK Installation Instructions - iOS **# 
If you are using CocoaPods (or Wish to use CocoaPods for integrating MogeanSDK), Please read Section A, otherwise jump to Section B

## **Section A: Using CocoaPods to Integrate MogeanSDK**
 ##
Step-1: Initiate CocoaPods $ pod init

Step-2: Integrate MogeanSDK Pod into Pod file. MogeanSDK is available as a private pod. Open your Podfile and add the following Sources source 'https://github.com/CocoaPods/Specs.git' source 'https://github.com/getmogean/MogeanSDK-iOS'
Add Target MogeanSDK and your podfile will look something like this:
  target 'AppTargetName' do 
    pod 'MogeanSDK', 
  end

Step-3: Install CocoaPod Install MogeanSDK $ pod install MogeanSDK is now integrated in your App.

## **Section - B: Without using CocoaPod** ##

Step-1: Clone this repository into your local system. Step-2: Drag and Drop MogeanSDK.framework into your workspace.

## **Section - C: Using MogeanSDK** ##
In your App Delegate, import MogeanSDK
import Mogean

Create a Shared Instance by calling: 
let mogeanSharedInstance:Mogean = Mogean.sharedInstance 
In your didFinishLaunchingWithOptions function, initialize Mogean by setting the MogeanID. 
mogeanSharedInstance.peelID = "<Your MogeanID Issued by Mogean>"
