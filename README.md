# CoinHive Miner Embed Template
This template allows you to easily embed the [CoinHive Miner](https://coinhive.com) into your own site to earn money without ads by letting your site visitors optionally mine Monero (a cryptocurrency similar to Bitcoin, Ether, etc.) using their CPU power by leaving the page open.

[Demo on my website](https://brandongiesing.com/cosimine/)

# UPDATE! (October 22nd, 2017)
CoinHive has released their own UI code finally and moved domains. This code is now split into two branches.

- `oldui`: The old widget extracted from their homepage (but updated to use AuthedMine). Doesn't have a user configible Speed option and is unsupported by me.
- `gh-pages`: This is the new "Simple UI" widget provided by CoinHive using AuthedMine. It's responsive UI is a bit better and it's officially supported by CoinHive and me.

Change your GH Pages branch to `oldui` in Settings if you want to continue to use the current UI with minimal changes. Use the default of `gh-pages` if you want the new UI or [switch to embedding the new UI itself](https://coinhive.com/documentation/simple-ui)

## Quick Start
1. Signup for [CoinHive](https://coin-hive.com/account/signup)
2. Once logged in, go to your [Sites & API Keys Settings](https://coinhive.com/settings/sites) and then copy the text next to `Site Key (public)`
3. Fork this GitHub Repo
4. Replace `UB0lonLFJXV0T5HYTiTcqgEJhcI9cxKW` in `index.html` with the key you copied above
5. Embed into your site with the following code (replace `USERNAME` with your GitHub username so for example, for me you would put `bgiesing`)

```html
<div class="codegena_iframe"><iframe src="https://USERNAME.github.io/CoinHiveMiner/index.html" height="255" width="442"  style="border:0px;float:middle;"></iframe></div><style>.codegena_iframe{position:relative;padding-bottom:32%;height:0;overflow: hidden;max-width:100%;}.codegena_iframe iframe{position:absolute;top:0;left:0;width:100%;height:100%;}</style>
```

Once you have it set up, you can optionally swap out the text, color scheme, and/or CoinHive logo with your own branding to make it fit better into your page. 

## Alternatives
The above 5 steps will get you up quickly but you don't have to do it exactly as mentioned above. I made this based around GitHub Pages to make it simple and work on sites that don't allow HTML page uploads with their own styling (common in CMSes like WordPress, Blogger, etc.) but there's other hosting options and ways to embed it if you prefer.

- Use CoinHive's embed directly in your site. Ideally you should be using that over this as is but this allows you to embed it in sites that only allow iFrames.
- Host it on your own server. If your host allows you to directly upload HTML files, you can just upload the `index.html` file to your site, rename it to something else (to not conflict with your website) and replace the full URL in the embed code above to the page.
- You also don't have to even embed it, just link the GitHub Pages URL directly.
- GitLab is another Git service that has page hosting

# Disclaimer/Credits
I'm not associated with CoinHive and this code is based heavily on their original code on their homepage. All I did was modualize it into simple embed and optimized the code to remove CSS/JS/IMGs that are no longer used after converting it.
