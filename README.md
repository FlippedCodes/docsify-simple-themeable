# Better Embed

A [docsify.js](https://github.com/docsifyjs/docsify) plugin to simplify the color selection for [docsify-themable](https://github.com/jhildenbiddle/docsify-themeable).

## Installation and usage instructions

> [!NOTE]
> Sorry for not providing a demo, but I thought this is a very self explanatory setup. But I am using this activly in [another projects](https://github.com/Karlo-Hosting/Docs/blob/a42df71978a439923162b411b2efb589df0a8e22/_css/colors-dark.css#L1).

How to install this plugin:

1. Make sure you have [docsify-themable](https://github.com/jhildenbiddle/docsify-themeable) installed.
2. Copy one of the stylesheet segments from below and copy it into the `head` section your `index.html` file. Make sure that is is after all other plugins and before your own modifications.
3. Copy the color-files from [the example directory](https://github.com/FlippedCodes/docsify-simple-themable/tree/main/example) into your projects `_css/` folder.
4. Change the colors in those files to your liking.

### Production

For production, please use the numbered version to prevent breaking changes in production.

``` html
<link rel="stylesheet" media="(prefers-color-scheme: dark)" href="./_css/colors-dark.css">
<link rel="stylesheet" media="(prefers-color-scheme: light)" href="./_css/colors-light.css">
<link rel="stylesheet" href="https://unpkg.com/docsify-simple-themable@1.0.0/dist/main.min.css">
```

### Development

If you are developing on a doc, you can use the latest. Make sure you switch it to production later, or the production one right away.

``` html
<link rel="stylesheet" media="(prefers-color-scheme: dark)" href="./_css/colors-dark.css">
<link rel="stylesheet" media="(prefers-color-scheme: light)" href="./_css/colors-light.css">
<link rel="stylesheet" href="https://unpkg.com/docsify-simple-themable@latest/dist/main.min.css">
```

## Tips

- This project is inspired by the color pallet naming scheme of [daisyUI](https://daisyui.com/): You can use their [theme generator](https://daisyui.com/theme-generator/) to select colors.
- If you think something on your docs should have a different color. You are more then welcome to copy the `src/main.css` into your `_css` folder as well. Just make sure you don't forget to adjust hte link in in the `head` section of your `index.html`!
- If you already have a css files, you are free to change the folder location in the stylesheet references in `index.html`.

## Contributing

I'm always happy, if someone has improvements to this little plugin. If you want to help, anything goes, but preferred is what is on the roadmap below or maybe discuss it as a GitHub issue first. ^^

### Roadmap

Nothing much here, but I'm planning to add the following features at some point:

- [ ] Remove requirement for docsify-themable.

## License

This repo is using the [MIT license](LICENSE).

## Credit

Thanks to the [docsify.js](https://docsify.js.org/#/) team to make changing CSS so simple. I usually don't front end, but this was a breeze to get working.
