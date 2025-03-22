<div align="center">

# ClearVision v7

IMAGE OUTDATED NEEDS UPDATING
![v6 Sapphire](https://i.imgur.com/U7UXrEN.png)

</div>


### Default presets
- Pearl - Pinkish theme, primarily for light mode
- Garnet - Magenta theme, primarily for dark mode
- Lapis - Darkish blue theme, primarily for dark mode | Art: https://www.pixiv.net/en/artworks/123209397 ; https://www.pixiv.net/en/users/44473246 -- NEED PERMISSION BEFORE USING
- Obsidian - Nearly black theme, primarily for dark mode | Art: https://www.publicdomainpictures.net/en/view-image.php?image=195779 ; CC0 ; https://www.publicdomainpictures.net/en/browse-author.php?a=1 (maybe?)
- Diamond - White theme, primarily for light mode

### Legacy Presets
Old ClearVision v6 presets are offered, too. All primarily for dark mode
- Sapphire - Darkish blue | Art: https://www.deviantart.com/kuldarleement/art/Stellar-collision-397866757 ; https://www.deviantart.com/kuldarleement/ ; http://www.kuldarleement.eu/  
- Ruby - Red | Art: https://www.deviantart.com/artistmef/art/Follow-the-path-279366207 ; https://www.deviantart.com/artistmef/  
- Amber - Orange | Art: https://www.deviantart.com/chromamancer/art/War-March-201045286 ; https://www.furaffinity.net/view/5408230 ; https://www.furaffinity.net/user/chromamancer/  
- Emerald - Green | Art: Work from "Guild Wars" or "Guild Wars 2" ; http://www.kekaiart.com/guild-wars-2.html ; http://www.kekaiart.com/uploads/5/4/7/6/5476798/7976137_orig.jpg ; http://www.kekaiart.com/t  
- Amethyst - Magenta | Art (tinted purple): https://www.deviantart.com/vityar83/art/gulls-149920115 ; https://www.deviantart.com/vityar83  
- Halloween - Orange, for festivity | Art: https://www.deviantart.com/unidcolor/art/Halloween-2014-491224711 ; https://www.deviantart.com/unidcolor/  
- Winter - Light blue, for festivity | Art: https://wall.alphacoders.com/big.php?i=114938 ; unknown artist.

Goals:
- Only supports visual refresh
- Supports both light and dark, along with dark variants
- Ensure all colour variables have some form of `calc(var(--saturation-factor,1) * $val)` in them
- Uses smallest css target possible
- Never use complex selectors before `> htmlElement` or `> *` without a very good reason
- Avoid usage of :has() without a good reason
- Always give reason for using `!important`
- Plugin support in extra files for respective client mods

### addons???

## Theme Editor

You can now customize the theme with a preview before downloading it to your computer.

Please keep in mind that **we do not manage the theme editor**, and cannot help with any bugs that come from using it.

> [Theme Editor](https://bdeditor.dev/theme/clearvision)

_Thank you to @Gibbu to providing this._

## Installing

Note: ClearVision doesn't actively support plugins (as in, we don't seek out and actively theme fixes to every new plugin). However, when a plugin is widely used, we try our best to stay compatible.

**For BD and Vencord:**

Download the theme file from [our official support server](https://clearvision.github.io/join), [the BetterDiscord Website](https://betterdiscord.app/theme/ClearVision) or [releases](https://github.com/ClearVision/ClearVision-v6/releases) and move it into your injector's themes folder:

- BetterDiscord: `%appdata%\betterdiscord\themes`
- Vencord: `%appdata%\vencord\themes`

**For using the theme online:**

There are multiple ways to do this if your client offers using an online version. The suggested two are `https://clearvision.github.io/ClearVision-v6/main.css` or `https://raw.githubusercontent.com/ClearVision/ClearVision-v6/master/ClearVision_v6.theme.css`

For customizing the theme from there, you'll want to use custom css and add any variables you'd like to change. It should look something like this

```
:root {
	--main-color: red;
	--hover-color: yellow;
}
```

## Building from source

To build the theme from source, first install npm from the dependencies below, then you can run `pnpm install` to install all missing dependencies and `pnpm run build` to compile the theme into the `/public` folder.

### Dependencies

- [NodeJS/npm](https://nodejs.org/)
- [pnpm](https://www.npmjs.com/package/pnpm)
- [sass](https://www.npmjs.com/package/sass)
- [PostCSS Autoprefixer](https://www.npmjs.com/package/autoprefixer)
- [PostCSS CLI](https://www.npmjs.com/package/postcss-cli)

## Contributing

_This section is outdated._

You can run `pnpm run test` to compile the theme.
The `main.css` file will be in the `/test` directory, which can then be copied into your client mod's Custom CSS or placed in the themes folder and enabled in settings. Just make sure any other themes are disabled for testing.
