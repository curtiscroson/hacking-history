# Setup

## Sublime Text

Download [Sublime Text 3](https://www.sublimetext.com/3) and install it for either Windows or OSX

Next, start Sublime Text 3 and then open the consol panel (Menu > View > Show Console). Now, install Sublime Text's plugin manager, called Package Control by copy/pasting the following command into Sublime's console.
``` ruby
import urllib.request,os,hashlib; h = 'df21e130d211cfc94d9b0905775a7c0f' + '1e3d39e33b79698005270310898eea76'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)
```

Next, we are going to set the Package Control settings to include all packages relevant to this class. To do this, open up Package Control's user settings (Menu > Sublime Text > Preferences > Package Settings > Package Control > User Settings). Copy/paste the following text, replacing any text that might already be there.
``` json
{
    "installed_packages":
    [
        "AdvancedNewFile",
        "Alignment",
        "All Autocomplete",
        "Anaconda",
        "AutoFileName",
        "BracketHighlighter",
        "Case Conversion",
        "Color Highlighter",
        "ColorPicker",
        "ConvertToUTF8",
        "CSS Extended Completions",
        "DocBlockr",
        "DocBlockr_Python",
        "Emmet",
        "Gist",
        "Git",
        "GitGutter",
        "Glue",
        "HTML Nest Comments",
        "HTML-CSS-JS Prettify",
        "JSHint",
        "JSHint Gutter",
        "LaTeXTools",
        "Local History",
        "Markdown Preview",
        "MarkdownEditing",
        "Material Theme",
        "Package Control",
        "Pretty JSON",
        "Quick File Open",
        "RegReplace",
        "SFTP",
        "SideBarEnhancements",
        "SublimeCodeIntel",
        "SublimeLinter",
        "Terminal",
        "Trimmer",
        "View In Browser",
        "Wget"
    ]
}
```

This will cause Sublime Text to start downloading these packages the next time you start the app. So, quit and restart Sublime Text. You will likely get a number of messages (including some error messages). You can close/ignore them for now. Once it has finished downloading (you can check the console to see), our last step is to configure Sublime's settings to use the package's correctly. To do that go Sublime's user settings (Menu > Preferences > Settings) and paste the following text, replacing any previous information.
``` json
{
    // If packages should be automatically upgraded when ST starts
    "auto_upgrade": true,
    // If missing packages should be automatically installed when ST starts
    "install_missing": true,
    // Material Theme
    "color_scheme": "Packages/Material Theme/schemes/Material-Theme.tmTheme",
    "theme": "Material-Theme.sublime-theme",
    // Indenting
    "tab_size": 4,
    "translate_tabs_to_spaces": true,
    "use_tab_stops": true,
    // Git
    "git_update_command": ["pull", "--ff", "--commit"],
    // Misc
    "ignored_packages":
    [
        "Vintage"
    ],   
    "rulers":
    [
        80
    ]
}
```