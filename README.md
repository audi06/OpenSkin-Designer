OpenSkin Designer
=================
[![GitHub release](https://img.shields.io/github/release/Humaxx/OpenSkin-Designer.svg)](https://github.com/Humaxx/OpenSkin-Designer/releases)
[![GitHub All Releases](https://img.shields.io/github/downloads/Humaxx/OpenSkin-Designer/total.svg)](https://github.com/Humaxx/OpenSkin-Designer/releases)
[![GitHub Releases (by Release)](https://img.shields.io/github/downloads/Humaxx/OpenSkin-Designer/3.2.3/total.svg)](https://github.com/Humaxx/OpenSkin-Designer/releases)

OpenSkin Designer is a further development of [e2skinner](https://code.google.com/p/e2skinner2/).

It includes a couple of new features i.e.:
* includes
* panels
* colored tree view
* screen search
* fold/unfold xml code
* quick add buttons (add screen, panel, widget, label, pixmap; delete item)
* simple autocomplete in code
* toggle conditional hiding element (show all, none, random, default)
* toggle markers (border indicators of elements)
* position replacement to 'center' disabled
* bugfixes
* etc.

## Notes
To view 'fMain.cs'[design] you have to delete the following lines 855-864 (they will autogenerated again...)
this.textBoxEditor2.Styles.BraceBad.FontName = "Verdana\0\0\0\0\0\0\0\0\0\0\0\0\0";
this.textBoxEditor2.Styles.BraceLight.FontName = "Verdana\0\0\0\0\0\0\0\0\0\0\0\0\0";
this.textBoxEditor2.Styles.CallTip.FontName = "Segoe UI\0\0\0\0\0\0\0\0\0\0\0\0";
this.textBoxEditor2.Styles.ControlChar.FontName = "Verdana\0\0\0\0\0\0\0\0\0\0\0\0\0";
this.textBoxEditor2.Styles.Default.BackColor = System.Drawing.SystemColors.InactiveBorder;
this.textBoxEditor2.Styles.Default.FontName = "Verdana\0\0\0\0\0\0\0\0\0\0\0\0\0";
this.textBoxEditor2.Styles.IndentGuide.FontName = "Verdana\0\0\0\0\0\0\0\0\0\0\0\0\0";
this.textBoxEditor2.Styles.LastPredefined.FontName = "Verdana\0\0\0\0\0\0\0\0\0\0\0\0\0";
this.textBoxEditor2.Styles.LineNumber.FontName = "Verdana\0\0\0\0\0\0\0\0\0\0\0\0\0";
this.textBoxEditor2.Styles.Max.FontName = "Verdana\0\0\0\0\0\0\0\0\0\0\0\0\0";

## Screenshots
<p align="center">
<img src="Screenshots/preview1.jpg?sanitize=true&raw=true" title="preview1" width="400"/>
<img src="Screenshots/preview2.jpg?sanitize=true&raw=true" title="preview2" width="400"/>
<img src="Screenshots/preview3.jpg?sanitize=true&raw=true" title="preview3" width="400"/>
</p>

## Changelog

### 3.2.0.0 (08.04.2019)
created by [Scrounger](https://github.com/Scrounger)
* Converter: support for 'FullDescription' added
* Resize picon on element size change
* Use attribute scale for ePixmap & widget which have 'pixmap' attribute.
* Converter MovieInfo added
* Show images for widgets with any render and 'path' attribute
* Show EventImage if render attribute contains 'eventimage'
* Show XHDPicon if render attribute contains 'xhdpicon'
* Show images with 'pixmaps' attribute

### 3.2.2.0 (08.04.2019 - 21.04.2019)
created by [Scrounger](https://github.com/Scrounger)
* cConverterSimplePresets added
* Alias font bug fixes -> gobal loading / usage added
* Fonts sorting added
* Label: font bug fix property grid -> change font or fontsize
* ListBox font added to property grid
* Show font style and size for listboxes
* Font bug fix -> catch exception if font is not defined or exist
* ListBox: Show entries added
* Label metrixreloadedvrunningtext added
* ListBox: count of entries to show bug fixed
* sAttributePixmap: element with attribute 'path' -> bug fix if skinPath is part of attribute path
* converterSimple.xml: MetrixReloaded converters added

### 3.2.3.0 (23.03.2020) by Humax
* Undefined colors are added alternatively ('#' is not replaced by 'un')'
* Added a option how to add undefined colors (with '#' or with 'un')
* Fixed unhandled exception if a borderset-file isn't existing
* Fixed unhandled exception in 'Windowstyle-preview' if no borderstyle is declared in skin.xml
* Bug fix in 'Windowstyle-preview': Now displaying correct borderset and filename
* Fixed a bug that probably exists since 3.1.0.3. Font preview is now again working
* Editor: now showing up to 99999 line numbers instead of max 999
* Editor: background color changed for better contrast
* Text-preview: using lcd.ttf if declared font is not found
* Added VTi-Fonts
* Converter bug fixes: 'TimeshiftService' added to prevent a exception in 'Timeshiftstate'
* Corrected xhdpicon.png for building in visual studio

### 3.2.3.1 (23.03.2020) by Humax
* Added more sources rendered as listbox
* Fixed unhandled exception if source = null

### 3.2.3.2 (26.03.2020) by Humax
* Fixed unhandled exception if no Font is declared or only alias - then using 'lcd.ttf'
* Fixed unhandled exceptions if a color is missing or declared with 'foregroundColors'
* Ask to show messageboxes again or not
* Bugfix: show picon also when a path is set
* Added option to set 'Fallback-Color', which is used for previewing some text

### 3.2.3.3 (27.03.2020) by Humax
* Fixed path not found exception
* Updated converter.xml
* Added speedyAXBlueRunningText
* Removed doubled attributs
* Added some entries to attribut-list like 'foregroundColors' 'options' 'pixmaps' and more
* Added a option to enable showing full attribut-list
* Autocomplete attribut list - max preview set to 15 instead of 5
### 3.2.3.4 (01.04.2020) by Humax
* Added render 'ChamaeleonRunningText'
* If pixmap have a path without specified filename, take random image
* Bugfix: pixmap path
* Added all renders containing 'runningtext'
* Handling all renders containing 'list' as listbox
* Notifying about unsafed changes