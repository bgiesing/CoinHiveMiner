# CoinHive Miner Embed Template
This template allows you to easily embed the [CoinHive Miner](https://coin-hive.com) into your own site to earn money without ads by letting your site visitors optionally mine Monero (a cryptocurrency similar to Bitcoin, Ether, etc.) using their CPU power by leaving the page open.

## Quick Start
1. Signup for [CoinHive](https://coin-hive.com/account/signup)
2. Once logged in, go to your [Sites & API Keys Settings](https://coin-hive.com/settings/sites) and then copy the text next to `Site Key (public)`
3. Fork this GitHub Repo
4. Replace `UB0lonLFJXV0T5HYTiTcqgEJhcI9cxKW` in `index.html` with the key you copied above
5. Embed into your site with the following code (replace `USERNAME` with your GitHub username so for example, for me you would put `bgiesing`)

```html
<div class="codegena_iframe"><iframe src="https://USERNAME.github.io/CoinHiveMiner/index.html" height="255" width="442"  style="border:0px;float:middle;"></iframe></div><style>.codegena_iframe{position:relative;padding-bottom:56.25%;height:0;overflow: hidden;max-width:100%;}.codegena_iframe iframe{position:absolute;top:0;left:0;width:100%;height:100%;}</style>
```

## More Options
The above 5 steps will get you up quickly but there's a few other things and alternatives you can do.

1. Swap out the text, color scheme, and/or CoinHive logo with your own branding to make it fit better into your page
2. Host somewhere else! I made this based around GitHub Pages to make it simple and work on sites that don't allow HTML page uploads with their own styling (common in CMSes like WordPress, Blogger, etc.) but if your host allows you, it would be better to upload the HTML file to your site and replace the full URL in the embed code above, not just the GitHub username.

# Disclaimer/Credits
I'm not associated with CoinHive and this code is based heavily on their original code on their homepage. All I did was modualize it into simple embed and optimized the code to remove CSS/JS/IMGs that are no longer used after converting it.
