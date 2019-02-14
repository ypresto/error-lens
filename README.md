# ErrorLens README

Welcome to ErrorLens.

ErrorLens enhances Visual Studio Code's inbuilt diagnostic highlighting. Visual Studio Code's default behavior for is to underline errors/warnings/info using a 'squiggly underline'. Whilst this is useful, it is sometimes possible to overlook errors and warnings.

ErrorLens turbo-charges the language diagnostic features, by making diagnostics stand out more prominently, highlighting the entire line wherever a diagnostic is generated by the language and also prints the diagnostic message(s) in-line at the site of the line of code which is generating the diagnostic.

![ErrorLens example](images/Screenshot-1.png)

## Features

* Lines containing errors or warnings or info are highlighted more obviously.
* Diagnostic descriptions are appended to the end of any line containing diagnostic info, meaning that you do not have to context-switch to the problem view.
* The status bar shows the number of diagnostics for the open file. (This can be configured)
* Settings can be configured to control the way ErrorLens displays enhanced diagnostics.
* Works for any language which provides diagnostics.

## Requirements

Built using Visual Studio Code 1.31.

Tested on Windows 10 (64-bit), Linux Mint & OSX 10.13.

## Extension Settings

This extension contributes the following settings:

* `errorLens.errorColor`: The background color used to highlight lines containing errors. (Alpha component can be used)
* `errorLens.errorTextColor`: The text color used to highlight lines containing errors. (Alpha component can be used)
* `errorLens.warningColor`: The background color used to highlight lines containing warnings. (Alpha component can be used)
* `errorLens.warningTextColor`: The text color used to highlight lines containing warnings. (Alpha component can be used)
* `errorLens.infoColor`: The background color used to highlight lines containing info. (Alpha component can be used)
* `errorLens.infoTextColor`: The text color used to highlight lines containing info. (Alpha component can be used)
* `errorLens.hintColor`: The background color used to highlight lines containing hints. (Alpha component can be used)
* `errorLens.hintTextColor`: The text color used to highlight lines containing hints. (Alpha component can be used)
* `errorLens.fontStyle`: Show ErrorLens annotations in Italics, or not?
* `errorLens.fontWeight`: Specifies the font weight for ErrorLens annotations.
* `errorLens.fontMargin`: Distance between end of the code line, and the start of the ErrorLens annotation. (CSS units)
* `errorLens.enabledDiagnosticLevels`: Customize which diagnostic levels to highlight.
* `errorLens.statusBarControl`: Customize how the VS Code Status Bar shows errors and warnings.
* `errorLens.addAnnotationTextPrefixes`: If 'true', prefixes the diagnostic severity ('Error:', 'Warning:' etc) to ErrorLens annotations.

## Extension Commands

This extension contributes the following commands:

* `ErrorLens.enable`: Enable ErrorLens.
* `ErrorLens.disable`: Disable ErrorLens.

## Contributing & contacting the author

The project is hosted on Github at: <https://github.com/phindle/error-lens>. Please submit suggestions, bug reports, Pull Requests and so on here.

I'm occasionally on Twitter @GeekyMcGeekface

## Known Issues

None known.

## Release Notes

Please refer to CHANGELOG.md for more details.

### 1.1.0

Second release of ErrorLens (February 2019).

*NOTE*: Configuration property `errorLens.errorMsgPrefix` has been removed. The reason is that this was somewhat unnecessary, and just added noise to the annotations. (cf. <https://github.com/phindle/error-lens/issues/9>)

### 1.0.0

Initial release of ErrorLens (October 2018)
