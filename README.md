# Color picker for Xamarin.Forms
Color picker control for Xamarin.Forms. It can be used as a large color mixer control (ColorPickerMixer) or as a dialog for select a color (ColorPickerDialog) or as an entry editor (ColorPickerEntry) of hexadecimal value with preview of a color and option of launch a dialog with color mixer.


## NuGet
* Available on NuGet: https://www.nuget.org/packages/Amporis.Xamarin.Forms.ColorPicker/ [![NuGet](https://img.shields.io/nuget/v/Amporis.Xamarin.Forms.ColorPicker.svg?label=NuGet)](https://www.nuget.org/packages/Amporis.Xamarin.Forms.ColorPicker/)


## Platform Support

Color picker control is written in C# (.NET 4.5) and uses standard Xamarin.Forms only.
Color picker was tested as NuGet in shared PCL library with these platforms:

|Platform|Version|
| ------------------- | :------------------: |
|Windows 10 UWP|10+|
|Xamarin.Android|API 14+|
|Xamarin.iOS|iOS 8+|


## License
Licensed under MIT license


## Usage

### ColorPickerDialog
```csharp
var color = await ColorPickerDialog.Show(MainGrid, "Choose color", Color.White, null);
```

**Parameters**
* **parent** (MainGird) - root container on the page, where a modal dialog will be temporarily placed
* **title** ("Choose color") - caption in the header of the dialog
* **defaultColor** (Color.White) - preselected color
* **settings** (null) - dialog settings - class ColorDialogSettings with these properties and its default values
  * BackgroundColor (#40000000)
  * DialogColor (#FFFFFFFF)
  * TextColor (#FF000000)
  * OkButtonText (OK)
  * CancelButtonText (Cancel)
  * DialogAnimation (true)
  * EditorsColor (#FFFFFFFF)
  * ColorPreviewBorderColor (#00FFFFFF)
  * SliderWidth (256)
  * ARGBEditorsWidth (65)
  * ColorEditorWidth (120)
  * EditAlfa (true)
