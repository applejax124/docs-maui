---
title: "Install Visual Studio 2022 to develop cross-platform apps using .NET MAUI"
description: "Learn how to install Visual Studio 2022 and Visual Studio 2022 for Mac, to develop native, cross-platform apps using .NET MAUI."
ms.date: 11/13/2023
monikerRange: ">=net-maui-8.0"
---

# Installation

Developing native, cross-platform .NET Multi-platform App UI (.NET MAUI) apps requires Visual Studio 2022 17.8 or greater, or Visual Studio 2022 for Mac 17.6.

<!-- markdownlint-disable MD025 -->
# [Visual Studio](#tab/vswin)
<!-- markdownlint-enable MD025 -->

To start developing native, cross-platform .NET MAUI apps on Windows, install Visual Studio 2022 17.8 or greater by following the [installation](#installation) steps.

## Prerequisites

- Visual Studio 2022 17.8 or greater. For information about supported operating systems, hardware, supported languages, and additional requirements and guidance, see [Visual Studio 2022 System Requirements](/visualstudio/releases/2022/system-requirements).

To build, sign, and deploy .NET MAUI apps for iOS, you'll also need:

- A Mac that is compatible with the latest version of Xcode. For more information, see Apple's [minimum requirements documentation](https://developer.apple.com/support/xcode/)
- The latest version of [Xcode](https://developer.apple.com/xcode).
- An [Apple ID](https://appleid.apple.com/account) and paid [Apple Developer Program](https://developer.apple.com/programs) enrollment. An Apple ID is required to deploy apps to devices, and to submit apps to the Apple Store.

Alternatively, to deploy debug builds of your app directly from Windows to your iOS device with [hot restart](~/ios/hot-restart.md), you'll need:

- An [Apple Developer account](https://appleid.apple.com/account) and paid [Apple Developer Program](https://developer.apple.com/programs) enrollment.

## Installation

1. To create .NET MAUI apps, you'll need the latest version of Visual Studio 2022:

    - [Download Visual Studio 2022 Community](https://c2rsetup.officeapps.live.com/c2r/downloadVS.aspx?sku=Community&channel=Release&Version=VS2022&source=VSLandingPage&add=Microsoft.VisualStudio.Workload.CoreEditor&add=Microsoft.VisualStudio.Workload.NetCrossPlat;includeRecommended&cid=2305)

    - [Download Visual Studio 2022 Professional](https://c2rsetup.officeapps.live.com/c2r/downloadVS.aspx?sku=Professional&channel=Release&Version=VS2022&source=VSLandingPage&add=Microsoft.VisualStudio.Workload.CoreEditor&add=Microsoft.VisualStudio.Workload.NetCrossPlat;includeRecommended&cid=2305)

    - [Download Visual Studio 2022 Enterprise](https://c2rsetup.officeapps.live.com/c2r/downloadVS.aspx?sku=Enterprise&channel=Release&Version=VS2022&source=VSLandingPage&add=Microsoft.VisualStudio.Workload.CoreEditor&add=Microsoft.VisualStudio.Workload.NetCrossPlat;includeRecommended&cid=2305)

1. Either install Visual Studio, or modify your existing installation, and install the .NET Multi-platform App UI development workload with its default optional installation options:

    :::image type="content" source="media/installation/vs/vs-workloads.png" alt-text="Visual Studio workloads for .NET MAUI.":::

<!-- markdownlint-disable MD025 -->
# [Visual Studio for Mac](#tab/vsmac)
<!-- markdownlint-enable MD025 -->

[!INCLUDE [Visual Studio for Mac end of life](~/includes/vsmac-eol.md)]

To start developing native, cross-platform .NET MAUI apps on macOS, install Visual Studio 2022 for Mac 17.6 by following the [installation](#installation) steps.

## Prerequisites

- Visual Studio 2022 for Mac 17.6. For information about supported operating systems, hardware, supported languages, and additional requirements and guidance, see [Visual Studio 2022 for Mac System Requirements](/visualstudio/releases/2022/mac-system-requirements).

To build, sign, and deploy .NET MAUI apps for iOS or macOS, you'll also need:

- A Mac that is compatible with the latest version of Xcode. For more information, see Apple's [minimum requirements documentation](https://developer.apple.com/support/xcode/)
- The latest version of [Xcode](https://developer.apple.com/xcode).
- An [Apple ID](https://appleid.apple.com/account) and paid [Apple Developer Program](https://developer.apple.com/programs) enrollment. An Apple ID is required to deploy apps to devices, and to submit apps to the Apple Store.

## Installation

1. To create .NET MAUI apps, you'll need the latest Visual Studio for Mac:

    > [!div class="button"]
    > [Download Visual Studio 2022 for Mac](https://visualstudio.microsoft.com/vs/mac/)

1. Either install Visual Studio 2022 for Mac, or modify your existing installation, and ensure that the following workloads are installed:

    - .NET
    - .NET MAUI
    - Android
    - iOS

    :::image type="content" source="media/installation/vsmac/mac-maui-workloads.png" alt-text="Visual Studio for Mac .NET MAUI workloads.":::
    :::image type="content" source="media/installation/vsmac/mac-legacy-workloads.png" alt-text="Visual Studio for Mac legacy workloads.":::

    > [!IMPORTANT]
    > For new installations of Visual Studio 2022 for Mac, selecting the .NET MAUI workload will automatically select the Android and iOS workloads, which are currently required for .NET MAUI development.

    <!-- At some point, the legacy workloads shouldn't be required. -->

1. Install .NET 8 through the [standalone installer](https://dotnet.microsoft.com/en-us/download/dotnet/8.0).
1. After .NET 8 has finished installing, run `dotnet workload install maui` in a terminal.

    [!INCLUDE [Enable .NET 8 support in Visual Studio Mac](includes/vsmac-net8.md)]

If you have network trouble while installing in a corporate environment, review the [installing behind a firewall or proxy](#installation-behind-a-firewall-or-proxy-server) instructions.

## Installation behind a firewall or proxy server

To install Visual Studio 2022 for Mac behind a firewall, certain endpoints must be made accessible in order to allow downloads of the required tools and updates for your software. For more information about configuring your network to allow access to the required endpoints, see [Install and use Visual Studio for Mac behind a firewall or proxy server](/visualstudio/mac/install-behind-a-firewall-or-proxy-server).

<!-- markdownlint-disable MD025 -->
# [Visual Studio Code (Preview)](#tab/visual-studio-code)
<!-- markdownlint-enable MD025 -->

> [!NOTE]
> .NET MAUI support in Visual Studio Code is still in preview. Try it out and [share your feedback](https://github.com/microsoft/vscode-dotnettools/issues)!

## Install Visual Studio Code and the .NET MAUI extension

1. Install [Visual Studio Code](https://code.visualstudio.com/).
1. In the Extensions tab, search for ".NET MAUI" and install the [.NET MAUI extension](https://aka.ms/mauidevkit-marketplace). The .NET MAUI extension automatically installs the [C# Dev Kit](https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.csdevkit) and [C#](https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.csharp) extensions, which are required for the .NET MAUI extension to run.  

    :::image type="content" source="media/installation/vscode/maui-extension-preview.png" alt-text="Screenshot of the Visual Studio Code extension pane showing the .NET MAUI extension":::

> [!NOTE]
> The .NET MAUI extension requires the C# Dev Kit and prerelease C# extensions. You must sign into C# Dev Kit to use the .NET MAUI extension's functionality. See [this blog post](https://devblogs.microsoft.com/visualstudio/announcing-csharp-dev-kit-for-visual-studio-code/) for more information about C# Dev Kit and its family of extensions.

## Set up .NET, .NET MAUI, and target platforms

To develop with .NET MAUI in Visual Studio code, you need to have .NET, the .NET MAUI workload, and a valid target platform based on your development machine's operating system:

| Your Operating System | Supported Target Platforms |
|---|---|
| Windows | Windows, Android |
| macOS | Android, iOS, macOS |
| Linux | Android |

### Windows

The recommended approach to setup your Windows machine for .NET MAUI development is through the Visual Studio installer. You can follow the instructions in the Visual Studio tab on this page to walk through installing the .NET MAUI workload. You can also use Visual Studio to manage different versions of Android, create emulators, update .NET and .NET MAUI, and more.

If you don't want to install Visual Studio, you can still get set up for .NET MAUI development by following these steps:

1. Install [.NET 8](/dotnet/core/install/windows).
1. After .NET has finished installing, run `dotnet workload install maui` in a terminal.
1. If you'd like to debug Android in Visual Studio Code, you also have to:
    1. Install [Microsoft OpenJDK 11](/java/openjdk/download#openjdk-11).
    1. Install the Android SDK. You can acquire the correct versions of the Android SDK and build tools by creating a new .NET MAUI project (`dotnet new maui`) and running the following command in your terminal:  
    `dotnet build -t:InstallAndroidDependencies -f:net8.0-android -p:AndroidSdkDirectory="<ANDROID SDK DIRECTORY>" -p:AcceptAndroidSDKLicenses=True`  
    On Windows, the suggested Android SDK directory value is `%LOCALAPPDATA%/Android/Sdk`.

> [!NOTE]
> See the [Troubleshooting > Android Setup](#android-setup) section for more information on setting up the Android SDK.

### macOS

1. Install [.NET 8](/dotnet/core/install/macOS).
1. Install the [latest stable Xcode](https://apps.apple.com/us/app/xcode/id497799835?mt=12).
1. After Xcode has finished installing, run `xcode-select --install` in a terminal to acquire the Xcode command line tools.
1. Run `dotnet workload install maui` in a terminal.
1. If you'd like to debug to Android in Visual Studio Code, you also have to:
    1. Install [Microsoft OpenJDK 11](/java/openjdk/download#openjdk-11).
    1. Install the Android SDK. You can acquire the correct versions of the Android SDK and build tools by creating a new .NET MAUI project (`dotnet new maui`) and running the following command in your terminal:  
    `dotnet build -t:InstallAndroidDependencies -f:net8.0-android -p:AndroidSdkDirectory="<ANDROID SDK DIRECTORY>" -p:AcceptAndroidSDKLicenses=True`  
    On macOS, the suggested Android SDK directory value is `$HOME/Library/Android/sdk`.

### Linux

1. Install [.NET 8](/dotnet/core/install/linux).
1. After .NET has installed, run `dotnet workload install maui-android` in a terminal.
1. If you'd like to debug to Android in Visual Studio Code, you also have to:
    1. Install [Microsoft OpenJDK 11](/java/openjdk/download#openjdk-11).
    1. Install the Android SDK from your preferred package manager, or from the [Android website](https://developer.android.com/about/versions/13/setup-sdk).

## Troubleshooting

You might face issues when setting up the .NET MAUI extension for Visual Studio Code. If you're still facing issues after following the below troubleshooting steps, please [report an issue](#provide-feedback).

### Project creation

If you try to create a new project and the file explorer keeps popping up in an infinite loop, you may not be selecting an empty folder. Check that there are no hidden files or folders, create a new folder, or create your .NET MAUI app from the command line using `dotnet new maui`.

### Android setup

There are multiple ways you can set up and manage Android SDKs on your machine:

* (Recommended) Use the [`dotnet build -t:InstallAndroidDependencies` target](#using-installandroiddependencies).
* Install via Visual Studio (Windows only).
* Install via Android Studio.
* Use the [Android Command Line Tools](https://developer.android.com/studio#command-tools).

No matter which way you install Android, you can develop .NET MAUI apps in Visual Studio Code. If the following troubleshooting steps don't solve your issue, please [Report a Problem](https://github.com/microsoft/vscode-dotnettools/issues).

#### Using "InstallAndroidDependencies"

* .NET 8 has a build target that helps set up your Android environment for you. You can add or remove the following properties to `dotnet build -t:InstallAndroidDependencies -f:net8.0-android` to configure your machine:
  * `-p:AndroidSdkDirectory "<PATH>"` installs or updates Android dependencies to the specified path (Note: You must use an absolute path without a tilde "~").
  * `-p:JavaSdkDirectory "<PATH>"` installs Java to the specified path (Note: You must use an absolute path without a tilde "~").
  * `-p:AcceptAndroidSDKLicenses=True` accepts the necessary Android licenses for development.

#### There's an error that the Android SDK or Java SDK was not found

* Open the command palette (Ctrl/Cmd + Shift + P) and search for the `.NET MAUI: Configure Android` command. Select both "Set Android SDK path" and "Set Android JDK path" and validate that they point to installations of each.
  * The Android SDK folder should have sub-folders such as `build-tools`, `cmdline-tools`, and `platform-tools`.
  * The Java OpenJDK folder should have sub-folders such as `bin`, `lib`, and more.
  * On Windows, if you install via Visual Studio, the Java SDK will be in `C:\Program Files\Microsoft\` and Android SDK will be in `C:\Program Files (x86)\Android\android-sdk`.
* Set the `JAVA_HOME` environment variable to a valid Java OpenJDK path.
* Set the `ANDROID_HOME` environment variable to your Android SDK path.
* Check your minimum versions of installed Android dependencies:
  * build-tools >= 32.0.0
  * cmdline-tools == 7.0
  * platforms;android-33*
  * .NET 7: platform-tools = 33.0.2
  * .NET 8: platform-tools = 34.0.1

#### There's an error that Android licenses aren't accepted

In an **elevated** command prompt or terminal, navigate to your Android SDK's `cmdline-tools/latest/bin/` folder and run `sdkmanager --licenses` then follow the CLI prompts.

#### My Android dependencies aren't loading in the Solution Explorer, but my app builds fine

This is a known issue if you install to `%APPDATA%` on Windows and will be fixed in a future release.

### iOS/Xcode Setup

* If you get an error that Xcode is not found, run `xcode-select --install` in a terminal, then check that `xcode-select -p` points to your Xcode installation.
* If you're still facing issues, open Xcode itself to make sure it loads correctly. Once Xcode is open, navigate to **Xcode > Settings > Locations** and check that the **Command Line Tools** field is pointing to the correct Xcode.
* There is a known issue that sometimes you have to build your iOS/macOS app twice for it to deploy. This will be fixed in an upcoming release.

### Debugging issues

* Debugging can fail to start for multiple reasons. If there isn't a clear error in the Output window, first double check that you are using the ".NET MAUI" run configuration in Visual Studio Code.
* You can try a command line build from the terminal to see if the error is with your code or the .NET MAUI extension. For example, you could run `dotnet build -f:net8.0-android` to see if your Android build succeeds outside of Visual Studio Code. If this build succeeds, please [Report an Issue](https://github.com/microsoft/vscode-dotnettools/issues)

## Known Limitations

This extension is still in early preview, so there are a number of known limitations. Please [give us your feedback](#provide-feedback) on other features you'd like to see as we continue building this new experience.

* XAML editing capabilities are very lightweight - you get basic syntax highlighting and autocomplete. We're exploring how to improve the XAML experience in a future release.
* Currently, you can't switch the target framework for IntelliSense (it will show syntax highlighting for only the first target framework listed in your .csproj file). This capability is in progress.
* XAML and .NET Hot Reload are't currently supported.
* This extension hasn't yet been fully tested with the latest iOS and Xcode betas.
Please [give us your feedback](#provide-feedback) on other features you'd like to see as we continue building this new experience!

## Provide Feedback

Please read the [C# Dev Kit FAQs](https://code.visualstudio.com/docs/csharp/cs-dev-kit-faq) and check existing [Known Issues](https://github.com/microsoft/vscode-dotnettools/issues) before filing a new issue or suggestion. You can file suggestions and issues from inside Visual Studio Code through through the **Help > Report Issue** dialog. Ensure you select “An extension” then the .NET MAUI extension in the drop-down.

:::image type="content" source="media/installation/vscode/report-issue.png" alt-text="Picture of the report issue dialog in Visual Studio Code":::

---

## Next steps

To learn how to create and run your first .NET MAUI app in Visual Studio 2022 on Windows, or Visual Studio 2022 for Mac, click the button below.

> [!div class="nextstepaction"]
> [Build your first app](first-app.md)
