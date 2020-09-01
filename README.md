1. Donwload OBS Tools.zip and unzip the file.
2. Add control panel: View/Panels/Browser panels. Add title in left column (ie. "Lower thirds"), put a path to file "lower thirds/control-panel.html" from the extracted folder into right column. Click "Apply" and close window. You can dock the panel between existing panels.
3. Add new browser source, pointing to file "lower thirds/browser-source.html". Set width to 1920 (or any other you use for streaming).
4. You can use predefined list - just click on the name - or type new data on the fly, then show them by clicking "Show". You can edit predefined values in "control-panel.html" file. Also you can change the logo. Basically, you can change everything, cause it's just a bunch of CSS lines :)

Tested only on PC, OBS 25.0+. I hope it'll run on Mac and Linux too.

It's just a working proof of concept, but works OK. I use simple transition, but you can do your own template and animate with CSS transitions, keyframes or whatever you want. For communication between control panel and browser layer I use BroadcastChannel API.

Panel color scheme is for OBS "Acri" theme, you can set your own colors in common/css/style-001.css (:root section).

Of course, there's a room for improvement: locked top panel, template system, animated SVG's as icons etc.
