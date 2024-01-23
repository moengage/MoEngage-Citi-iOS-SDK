![Logo](https://github.com/moengage/MoEngage-iOS-SDK/blob/master/Images/moe_logo_blue.png)
# MoEngage-iOS-SDK

MoEngage provides a platform which enables companies to deliver personalized interactions to their users through push notifications, in-app campaigns, email campaigns and other re-targeting channels.

## Integration

To install the framework manually, follow the guide https://developers.moengage.com/hc/en-us/articles/4404183451412-Manual-Integration

## SDK Initialization

Login to your MoEngage account, go to **Settings** in the left panel of the dashboard. Under App Settings, you will find your **APP ID**. Provide this APP ID while initializing the SDK with **initializeDefaultTestInstanceWithConfig:** and **initializeDefaultLiveInstanceWithConfig:** methods as shown below.

### In Objective-C:

    @import MoEngageSDK;
    
    - (BOOL)application:(UIApplication *)application didFinishLaunchingWithOptions:(NSDictionary *)launchOptions {
       //TODO: Add your MoEngage App ID and Data center.
       MoEngageSDKConfig* sdkConfig = [[MoEngageSDKConfig alloc] initWithAppId:@"YOUR APP ID" dataCenter: DATA_CENTER];
       
       // MoEngage SDK Initialization
       // Separate initialization methods for Dev and Prod initializations
       #ifdef DEBUG
         [[MoEngage sharedInstance] initializeDefaultTestInstance:sdkConfig];
       #else
         [[MoEngage sharedInstance] initializeDefaultLiveInstance:sdkConfig];
       #endif
    
       //Rest of the implementation of method
       //-------
    }

### In Swift:

    import MoEngageSDK
    
    func application(_ application: UIApplication, didFinishLaunchingWithOptions launchOptions: [UIApplicationLaunchOptionsKey: Any]?) -> Bool {
  
      //Add your MoEngage App ID and Data center.
      let sdkConfig = MoEngageSDKConfig(appId: "YOUR APPID", dataCenter: DATA_CENTER);
 
      // MoEngage SDK Initialization
      // Separate initialization methods for Dev and Prod initializations
      #if DEBUG
          MoEngage.sharedInstance.initializeDefaultTestInstance(sdkConfig)
      #else
         MoEngage.sharedInstance.initializeDefaultLiveInstance(sdkConfig)
      #endif
 
      //Rest of the implementation of method
      //-------
      return true
    }


Thats it!! SDK is successfully integrated and initialized in the project, and ready to use. 

## Developer Docs
Please refer to our developer docs to know how to make use of our SDK to track Events and User Attributes, to implement Push Notification and InApps: [link](https://docs.moengage.com/docs/sdk-integration).

## Change Log
See [SDK Change Log](https://github.com/moengage/MoEngage-iOS-SDK/blob/master/CHANGELOG.md) for information on every released version.

## Support
For any issues you face with the SDK and for any help with the integration contact us at `support@moengage.com`.
