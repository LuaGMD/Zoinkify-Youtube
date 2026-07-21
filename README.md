<div align = center>

# Zoinkify

Is your browser experience boring? Are you having  
trouble finding engaging click-baity videos?

**Fear no more.**

This extension adds the famous  
youtuber **Zoink** to every thumbnail.


</div>

## Notes

- This extension should be compatible with any Firefox / Chromium based browser.
- This extension was inspired by **[MagicJinn][UI Youtube]** and his **[Extension][UI Website]**.
- This extension is unofficial and not affiliated with MrBeast or YouTube.

## Making your own

Want to customize this extension with a different YouTuber or personality? Here's how:

1. **Fork this repository** and or clone it to your local machine
2. **Replace the images**: 
   - Replace the images in the `images/` folder with your own (numbered sequentially: `1.png`, `2.png`, `3.png`, etc. Leave no gaps in the numbering.) You can use websites such as [Photoroom](https://www.photoroom.com/tools/background-remover) to remove the background of your images, and websites like [compresspng](https://compresspng.com/) to compress your images.
   - Update `icon.png` with your own icon
3. **Update the manifest**:
   - Edit `manifest.json` and `manifest v3.json` to change the extension name, version number and description
4. **Handle text images** (optional):
   - If any images contain text that shouldn't be flipped, add them to `images/flip_blacklist.json`
   - Create alternative flipped versions in `images/textFlipped/` if needed
   - If you have no use for the flip blacklist, you should delete the `flip_blacklist.json` file.
5. **Test locally**: Load the extension in developer mode in your preferred browser. This is important. Do not upload broken extensions!
6. **Build the extension**: If you have 7-Zip installed, run `build.bat` to build the extension. This will create a zip file in the root directory of the repository. (The 7-Zip dependency is unfortunately required because Windows' built in Compress-Archive feature is completely busted for some reason). If packing manually, only include `images/`, `manifest.json`, `icon.png`, `settings.html`, `settings.js` and `mrbeastify.js`. When packing for Chrome, use the `manifest v3.json` file, but rename it to `manifest.json`.
7. **Upload to extension stores**: You can upload your customized version to Chrome Web Store, Firefox Add-ons, etc.



[UI YouTube]: https://www.youtube.com/@magicjinn
[UI Website]: https://chromewebstore.google.com/detail/youtube-mrbeastify/dbmaeobgdodeimjdjnkipbfhgeldnmeb
