<!-- Please do not edit this file. Edit the `blah` field in the `package.json` instead. If in doubt, open an issue. -->


# `$ google-font-downloader`

 [![Support me on Patreon][badge_patreon]][patreon] [![Buy me a book][badge_amazon]][amazon] [![PayPal][badge_paypal_donate]][paypal-donations] [![Ask me anything](https://img.shields.io/badge/ask%20me-anything-1abc9c.svg)](https://github.com/IonicaBizau/ama) [![Version](https://img.shields.io/npm/v/google-font-downloader.svg)](https://www.npmjs.com/package/google-font-downloader) [![Downloads](https://img.shields.io/npm/dt/google-font-downloader.svg)](https://www.npmjs.com/package/google-font-downloader)

> Download Google fonts by providing the url

#### Usage


You can use this tool to download Google Fonts for offline use, just by providing the Google APIs url.


:bulb: **Note**: It's not clear yet if Google Fonts are EU GDPR compliant (see [this issue](https://github.com/google/fonts/issues/1495)). This may be a good reason to download the Google Fonts you use on your server.

#### How it works


You need to provide the url to the Google APIs endpoint (e.g. `https://fonts.googleapis.com/css?family=Open+Sans:400,400i,700,700i`) and you will get the following files/directories in the current working directory:


 - A file named `google-fonts-<timestamp>.css`—this will contain the CSS snippets that you need to copy in your app. You may need to update the paths to the font files.
 - A directory structure looking like this: `fonts/<font-name>/<version>/<font-file>`

![Example](https://i.imgur.com/yGcOPKg.gif)

## :cloud: Installation

You can install the package globally and use it as command line tool:


```sh
# Using npm
npm install --global google-font-downloader

# Using yarn
yarn global add google-font-downloader
```


Then, run `google-font-downloader --help` and see what the CLI tool can do.


```
$ google-font-downloader --help
Usage: google-font-downloader <url> [options]

Download Google fonts by providing the url

Command arguments:
  <url>  The Google APIs url.

Options:
  -v, --version  Displays version information.
  -h, --help     Displays this help.

Examples:
  $ google-font-downloader https://fonts.googleapis.com/css?family=Open+Sans:400,400i,700,700i

Documentation can be found at https://github.com/IonicaBizau/google-font-downloader#readme.
```

## :yum: How to contribute
Have an idea? Found a bug? See [how to contribute][contributing].


## :sparkling_heart: Support my projects

I open-source almost everything I can, and I try to reply everyone needing help using these projects. Obviously,
this takes time. You can integrate and use these projects in your applications *for free*! You can even change the source code and redistribute (even resell it).

However, if you get some profit from this or just want to encourage me to continue creating stuff, there are few ways you can do it:

 - Starring and sharing the projects you like :rocket:
 - [![Buy me a book][badge_amazon]][amazon]—I love books! I will remember you after years if you buy me one. :grin: :book:
 - [![PayPal][badge_paypal]][paypal-donations]—You can make one-time donations via PayPal. I'll probably buy a ~~coffee~~ tea. :tea:
 - [![Support me on Patreon][badge_patreon]][patreon]—Set up a recurring monthly donation and you will get interesting news about what I'm doing (things that I don't share with everyone).
 - **Bitcoin**—You can send me bitcoins at this address (or scanning the code below): `1P9BRsmazNQcuyTxEqveUsnf5CERdq35V6`

    ![](https://i.imgur.com/z6OQI95.png)

Thanks! :heart:



## :scroll: License

[MIT][license] © [Ionică Bizău][website]

[badge_patreon]: http://ionicabizau.github.io/badges/patreon.svg
[badge_amazon]: http://ionicabizau.github.io/badges/amazon.svg
[badge_paypal]: http://ionicabizau.github.io/badges/paypal.svg
[badge_paypal_donate]: http://ionicabizau.github.io/badges/paypal_donate.svg
[patreon]: https://www.patreon.com/ionicabizau
[amazon]: http://amzn.eu/hRo9sIZ
[paypal-donations]: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=RVXDDLKKLQRJW
[donate-now]: http://i.imgur.com/6cMbHOC.png

[license]: http://showalicense.com/?fullname=Ionic%C4%83%20Biz%C4%83u%20%3Cbizauionica%40gmail.com%3E%20(https%3A%2F%2Fionicabizau.net)&year=2018#license-mit
[website]: https://ionicabizau.net
[contributing]: /CONTRIBUTING.md
[docs]: /DOCUMENTATION.md
