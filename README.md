# ![LOGO](logo.png) RiteKit **flow**ground Connector

## Description

A generated **flow**ground connector for the RiteKit API (version 1.0.0).

Generated from: https://api.apis.guru/v2/specs/ritekit.com/1.0.0/swagger.json<br/>
Generated at: 2019-05-07T17:43:54+03:00

## API Description

RiteKit API is based on REST principles.

Authentication uses standard OAuth 2.0 process

##Getting started

1. Sign up for [RiteKit](https://ritekit.com/)

1. Go to [developer dashboard](https://ritekit.com/developer/dashboard/)

1. Click "Create a token" button to get your **Client ID** and **Client secret**

1. When you reach your free limit of calls per month, [upgrade to paid tiers](https://ritekit.com/developer/)

## Options for authorizing API Calls

#### Using Client ID directly

You can directly connect to our API using your **client ID** by sending it as a GET query parameter. This option is simple (no need for oAuth) but it should be used only in case the Client ID is not exposed publicly.

GET  https://api.ritekit.com/v1/stats/multiple-hashtags?tags=php&client_id=292c6912e7710c838347ae178b4a

## Authorization

This API does not require authorization.

## Actions

### Auto-Emojify

> Returns text of the post with emoji added

#### Input Parameters
* `text` - _required_ - Text of the post

### Emoji Suggestions

> Returns list of emoji suggestions for a given text of the post

#### Input Parameters
* `text` - _required_ - Text of the post

### Animate Image

> Returns URL of an animated GIF.

#### Input Parameters
* `url` - _required_ - URL of the company
* `type` - _required_ - URL of the company

### Company Logo

> Returns a company logo based on website domain. If the logo is not in our database yet, it will be extracted from the site on the fly. White logo background is automatically removed to make the logo look better on color backgrounds.

#### Input Parameters
* `domain` - _required_ - URL of the company

### Text to Image

> Returns URL of an image created from text according to given style parameters

#### Input Parameters
* `quote` - _required_ - Text of the quote
* `author` - _required_ - Name of the author/source
* `fontSize` - _required_ - Font size for the quote (author font size is calculated automatically)
* `quoteFont` - _required_ - Font-family used for quote text
* `quoteFontColor` - _required_ - Font color of the quote text
* `authorFont` - _required_ - Font-family used for author name
* `authorFontColor` - _required_ - Font color of the author
* `enableHighlight` - _required_ - Enable highlight on quote text
* `highlightColor` - _required_ - Color used for highlight
* `bgType` - _required_ - Background type (gradient/solid)
* `backgroundColor` - _required_ - Background color for solid background type
* `gradientType` - _required_ - Type of gradient background (linear/radial)
* `gradientColor1` - _required_ - First color for gradient background type
* `gradientColor2` - _required_ - Second color for gradient background type
* `brandLogo` - _required_ - URL of the brand logo
* `animation` - _required_ - Animation type: none, rays, glint, circle
* `showQuoteMark` - _optional_ - showing/hiding quote mark

### List of CTAs

> Returns list of available CTA for current user. Requires each user to authenticate with RiteKit

### Shorten Link

> Returns a shorten link with a given CTA.

#### Input Parameters
* `url` - _required_ - URL
* `cta` - _required_ - cta id

### Trending Hashtags

> Returns list of hashtags currently trending on Twitter

#### Input Parameters
* `green` - _optional_ - Restrict results only to green hashtags. Hides overused (red) hashtags.
* `latin` - _optional_ - Restrict results only to hashtags with latin characters

### Auto-Hashtag

> Returns auto-hashtagged text of the post.

#### Input Parameters
* `post` - _required_ - Text of the post
* `maxHashtags` - _optional_ - Max number of hashtags.
* `hashtagPosition` - _optional_ - Position of hashtags: end => at the end, auto => anywhere

### Hashtag Suggestions

> Returns list of hashtag suggestions for a single-word topic or a shorter text up to 1000 characters. Takes into account both semantic relevancy and real-time hashtag popularity.

#### Input Parameters
* `text` - _required_ - Topic

### Hashtag History

> Returns historical stats for a given hashtag from the last 30 days

#### Input Parameters
* `hashtag` - _required_ - Hashtag without # mark

### Hashtag Stats

> Returns real-time stats for up to 100 hashtags (updated hourly).

#### Input Parameters
* `tags` - _required_ - Hashtag(s) without # mark

### Hashtags cleaner

> Remove banned hashtags before posting to Instagram

#### Input Parameters
* `post` - _required_ - post

## License

**flow**ground :- Telekom iPaaS / ritekit-com-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
