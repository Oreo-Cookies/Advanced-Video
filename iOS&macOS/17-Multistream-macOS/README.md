# 17 Multistream

*其他语言版本： [简体中文](README.zh.md)*

The Large Group Video Chat macOS Sample App is an open-source demo that will help you get a large group video chat using the Agora Video SDK.

With this sample app, you can:

- Join / leave channel
- Mute / unmute audio
- Mute / unmute remote audio and video
- Group video chat up to 17 people

## Prerequisites

- Xcode 10.0+

## Quick Start

This section shows you how to prepare, build, and run the sample application.

### Obtain an App Id

To build and run the sample application, get an App Id:

1. Create a developer account at [agora.io](https://dashboard.agora.io/signin/). Once you finish the signup process, you will be redirected to the Dashboard.
2. Navigate in the Dashboard tree on the left to **Projects** > **Project List**.
3. Save the **App Id** from the Dashboard for later use.
4. Generate a temp **Access Token** (valid for 24 hours) from dashboard page with given channel name, save for later use.

5. Open `17-Multistream.xcodeproj` and edit the `KeyCenter.swift` file. Update `<#Your App Id#>` with your App Id, and assign the token variable with the temp Access Token generated from dashboard.

    ``` Swift
    static let AppId: String = <#Your App Id#>
    // assign token to nil if you have not enabled app certificate
    static var Token: String? = <#Temp Access Token#>
    ```

### Integrate the Agora Video SDK

1. Download the [Agora Video SDK](https://www.agora.io/en/download/). Unzip the downloaded SDK package and copy the following files from the SDK `libs` folder into `iOS&macOS/libs/macOS` folder.

    - `AograRtcKit.framework`
    - `AgoraRtcCryptoLoader.framework`
    - `libcrypto.a`

2. pod install, create 17-Multistream.xcworkspace.
  
3. Open Xcode and run this project.

## Contract Us

- For potential issues, you may take a look at our [FAQ](https://docs.agora.io/en/faq) first
- Dive into [Agora SDK Samples](https://github.com/AgoraIO) to see more tutorials
- Would like to see how Agora SDK is used in more complicated real use case? Take a look at [Agora Use Case](https://github.com/AgoraIO-usecase)
- Repositories managed by developer communities can be found at [Agora Community](https://github.com/AgoraIO-Community)
- You can find full API document at [Document Center](https://docs.agora.io/en/)
- If you encounter problems during integration, you can ask question in [Developer Forum](https://stackoverflow.com/questions/tagged/agora.io)
- You can file bugs about this sample at [issue](https://github.com/AgoraIO/Advanced-Video/issues)

## License

The MIT License (MIT).
