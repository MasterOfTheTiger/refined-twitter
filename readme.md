# <img src="source/icon.png" width="45" align="left">Reimagined Twitter (Refined Twitter for Firefox)

> Browser extension that simplifies the Twitter interface and adds useful features for Firefox

This project is forked from [Refined Twitter](https://github.com/sindresorhus/refined-twitter). This project will tweak a few things (because people have differing tastes) and is be a Firefox Addon.
[![XO code style](https://img.shields.io/badge/code_style-XO-5ed9c7.svg)](https://github.com/xojs/xo) [![Gitter](https://badges.gitter.im/join_chat.svg)](https://gitter.im/refined-twitter/Lobby)

We use Twitter a lot and notice many dumb annoyances we'd like to fix. So here be dragons.

**Read the [blog post](https://blog.sindresorhus.com/refined-twitter-74038424fe2a) and discuss it on [Product Hunt](https://www.producthunt.com/posts/refined-twitter)**

If you use any browser but Firefox, refer [here](https://github.com/sindresorhus/refined-twitter)

## Install

- **Firefox** add-on: Get it here: https://addons.mozilla.org/en-US/firefox/addon/reimagined-twitter/


## Highlights

- Simplified and improved UI.
- Hides promoted tweets.
- Auto-loads new tweets in the stream if you're scrolled to the top. No more clicking `See 3 new Tweets`!
- Fixes the file extension when saving images in tweets. No more `foo.jpg_large`!
- Uses the system font.
- [Embeds the photo from Instagram links directly in the tweet.](https://user-images.githubusercontent.com/170270/34315380-12d52994-e77f-11e7-8e23-27b76aee4df2.png)
- Improves performance. <sup>[1](https://github.com/sindresorhus/refined-twitter/pull/14)</sup> <sup>[2](https://github.com/sindresorhus/refined-twitter/commit/23897e251d2bc8d59526129ce54c7a5bf1ef884c)</sup>
- Hides "Liked" tweets in the stream.
- [Hides "And others follow" tweets in the stream.](https://user-images.githubusercontent.com/5341072/39945031-cc81125a-5560-11e8-8334-ea310a9dfdad.png)
- [Syntax highlighting in code blocks.](https://github.com/sindresorhus/refined-twitter/issues/37)
- [Adds Markdown-like styling of `text wrapped in backticks`.](https://user-images.githubusercontent.com/12901172/38168571-d9bd82ea-351d-11e8-9858-0d7c8993cdd3.png)
- Uses the original image in tweet image galleries instead of a downsized version.
- [Removes the annoying suggestions in the search popover.](https://user-images.githubusercontent.com/170270/33800304-70198358-dd3d-11e7-9870-477a44f74f4d.png)
- Hides "Notifications" activity for new followers and being added to a list.
- Preserves unsent text in the Messages modal when it closes.
- Highlight your mentions in the stream.
- [Adds a `Likes` button to the main navbar.](https://user-images.githubusercontent.com/14620121/35988497-ace9f93e-0ce5-11e8-8675-17e6ee38cd99.png)
- Keyboard shortcut to toggle Night Mode (<kbd>Alt</kbd><kbd>m</kbd>).
- Uses your personal color theme on all profiles.
- Hides the header image on profile pages.
- [Shows alternative image text below images when available.](https://user-images.githubusercontent.com/170270/40556400-b46c292c-6076-11e8-8241-f5c4e1a7a161.png)

Tip: Twitter has a native [dark mode](https://github.com/sindresorhus/refined-twitter/issues/10) and you can toggle it using <kbd>Ctrl</kbd><kbd>m</kbd>. And press <kbd>Shift</kbd> <kbd>?</kbd> to see all keyboard shortcuts.

<img src="media/screenshot.gif" width="1272">


## Customization

We are happy for suggestions and contributions. But there are things that won't be changed.

This doesn't necessarily limit you from manually disabling functionality that is not useful for you. Options include:

1. *(CSS Only)* Use a Chrome extension that allows injecting custom styles into sites, based on a URL pattern. [Stylish](https://chrome.google.com/webstore/detail/stylish/fjnbnpbmkenffdnngjfgmeleoegfcffe?hl=en) is one such tool. [Example](https://github.com/sindresorhus/refined-github/issues/136#issuecomment-204072018)

2. Clone the repository, make the adjustments you need, and [load the unpacked extension in Chrome](https://developer.chrome.com/extensions/getstarted#unpacked), rather than installing from the Chrome Store.


## Contribute

Suggestions and pull requests are highly encouraged!

In order to make modifications to the extension you'd need to run it locally.

Please follow the below steps:

```sh
git clone https://github.com/MasterOfTheTiger/reimagine-twitter
cd reimagine-twitter
npm install    # Install dev dependencies
npm run build  # Build the extension code so it's ready for the browser
npm run watch  # Listen for file changes and automatically rebuild
```

Once built, load it in the browser of your choice:

<table>
	<tr>
		<th>Chrome</th>
		<th>Firefox</th>
	</tr>
	<tr>
		<td width="50%">
			<ol>
				<li>Open <code>chrome://extensions</code>
				<li>Check the <strong>Developer mode</strong> checkbox
				<li>Click on the <strong>Load unpacked extension</strong> button
				<li>Select the folder <code>reimagine-twitter/extension</code>
			</ol>
		</td>
		<td width="50%">
			<ol>
				<li>Open <code>about:debugging#addons</code>
				<li>Click on the <strong>Load Temporary Add-on</strong> button
				<li>Select the file <code>reimagine-twitter/extension/manifest.json</code>
			</ol>
		</td>
	</tr>
</table>


## Related

- [Refined GitHub](https://github.com/sindresorhus/refined-github) - GitHub version of the original extension


## Maintainers

### For Refined Twitter
- [Sindre Sorhus](https://github.com/sindresorhus)
- [Filipe Kiss](https://github.com/filipekiss)
- [Jorge Gonzalez](https://github.com/jorgegonzalez)

### For Reimagined Twitter
- [MasterOfTheTiger](https://github.com/MasterOfTheTiger)


## License

MIT
