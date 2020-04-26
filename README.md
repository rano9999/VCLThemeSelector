# VCLThemeSelector [![License](https://img.shields.io/badge/License-Apache%202.0-yellowgreen.svg)](https://opensource.org/licenses/Apache-2.0)

**Easy and elegant preview/selection of Theme (Light/Dark/Other) for VCL apps plus HighDPI demo**

With VCLThemeSelector you can easily add a modern and elegant Theme selector for your Delphi VCL app. The Form shows all the VCL Styles included in your application, then arrange them in defined Rows and Columns. You can specify to include or not 'Windows' not-styled option.

![https://github.com/EtheaDev/VCLThemeSelector/blob/master/Demo/Images/Preview3x3.jpg](https://github.com/EtheaDev/VCLThemeSelector/blob/master/Demo/Images/Preview3x3.jpg)

Example:

```pascal
var
  LActiveStyleName: string;
  LExcludeWindows: boolean;
  LMaxRows, LMaxCols: Integer;
begin  
  LActiveStyleName := TStyleManager.ActiveStyle.Name;
  LExcludeWindows := False;
  LMaxRows := 3;
  LMaxCols := 3;
  if ShowVCLThemeSelector(LActiveStyleName, LExcludeWindows, LMaxRows, LMaxCols) then
    TStyleManager.SetStyle(LActiveStyleName);
end;    
```

License: the CBVCLStylePreview is based on VCLStylePreview (Vcl.Styles.Ext) from:
[github.com/RRUZ/vcl-styles-utils](https://github.com/RRUZ/vcl-styles-utils/) and includes High-DPI support, and released under Apache 2.0 license.

## High-DPI Delphi App full example ##

Also included in this repository you can find a full example of an HighDPI - VCL Themed enabled application that uses the VCLThemeSelector to change the Theme. You can run the demo from: Demo\Bin\SplitViewDemo.exe.

![https://github.com/EtheaDev/VCLThemeSelector/blob/master/Demo/Images/DemoPreview.jpg](https://github.com/EtheaDev/VCLThemeSelector/blob/master/Demo/Images/DemoPreview.jpg)

License: this Demo is inspired by TSplitView demo (original software is Copyright (c) 2015 Embarcadero Technologies, Inc.) and is released under Apache 2.0 license.

WARNING: to edit and compile the demo you must first download:
[IconFontsImageList free components here...](https://github.com/EtheaDev/IconFontsImageList/)

Feedback are welcome!
