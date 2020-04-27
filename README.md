# TranscoderXamarin [![NuGet](https://img.shields.io/nuget/v/TranscoderXamarin.svg)](https://www.nuget.org/packages/TranscoderXamarin)

TranscoderXamarin is Xamarin Binding for https://github.com/natario1/Transcoder Project.

## Installation
Install Nuget in Android Project

**IMPORTANT**

Install [Xamarin.Kotlin.StdLib.Jdk7](https://www.nuget.org/packages/Xamarin.Kotlin.StdLib.Jdk7/) since this is a dependency binding over Kotlin library

## Usage

Implement interface in the class you are using Transcoder

```chsarp
public YourClass : Java.Lang.Object, ITranscoderListener
{
		//Your Code
}
```

For transcoding files

```chsarp
var transcoder = Transcoder
                .Into(destination)
                .AddDataSource(trim)
                .SetVideoTrackStrategy(videoStrategy)
                .SetAudioTrackStrategy(audioStrategy)
                .SetListener(this)
                .Transcode();
```

For more information about the usage of library, visit original library documentation https://natario1.github.io/Transcoder/

##Credits
Thanks @natario1 for the awesome original library.

If this binding was useful or saved your time, mind buying me a coffee?
<a href="https://www.buymeacoffee.com/muhaym" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" style="height: 51px !important;width: 217px !important;" ></a>
