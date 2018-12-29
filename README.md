# SimpleXam.TintedImagePlugin

This plugin is designed to overlay the colour of the selected image with one specific fill colour. This should be primarily used with single-colour icons and/or images. This is an extension from the `Image`.

## Implementation

C#:
```c#
    using SimpleXam.TintedImagePlugin;
    
    ...

    TintedImage circleView = new TintedImage()
    {
        Source = "myImage.png",
        Tint = Xamarin.Forms.Color.Blue
    };
```
XAML:

```xml
    <ContentPage 
        xmlns="http://xamarin.com/schemas/2014/forms"
        xmlns:x="http://schemas.microsoft.com/winfx/2009/xaml"
        xmlns:tint="clr-namespace:SimpleXam.TintedImagePlugin;assembly=SimpleXam.TintedImagePlugin"
        x:Class="MyApp.MainPage">
        <StackLayout>
            <tint:TintedImage
                Source="myImage.png"
                Tint="Blue" />
        </StackLayout>
    </ContentPage>
```
