# subliminal-stata - Sublime Text syntax highlighting for Stata

## Use
  - The **.tmLanguage** and **.tmTheme** files can be used to customize syntax highlighting for Stata in Sublime Text.
  - **Stata.tmLanguage** controls syntax definitions for Stata code.
    - This file format is comparable to a **.sublime-syntax** file.
  - The **Stata-[Dark|Light].tmTheme** files control the color scheme for Stata code.
    - These files are comparable to **.sublime-color-scheme** files.
    - There are two color schemes: dark and light.
  - The sytnax highlighting will affect scripts with the file extensions: __.do__ and __.ado__.

## Integration
  - The files should be placed in the User Package directory.
    - In Sublime Text 3, this directory may be located here:
      - C:\Users\[NAME]\AppData\Roaming\Sublime Text 3\Packages\User
  - To select the dark or light theme, update **Stata.sublime-settings** to point to the matching **Stata-[Dark|Light].tmTheme** file.
    - Alternately, this can accomplished with a .do or .ado file as the active script in Sublime Text by navigating to:
      - Preferences --> Settings - Syntax Specific
      - Update the `color_scheme` parameter in the right-hand window to point to the correct **.tmTheme** file.
      ` { `
      `   "color_scheme": "Packages/User/Stata-Dark.tmTheme" `
      ` } `

## Acknowledgements
The syntax highlighting files build off Stata Enhanced, available through Package Control.
  - https://packagecontrol.io/packages/Stata%20Enhanced
  - https://github.com/andrewheiss/SublimeStataEnhanced 
