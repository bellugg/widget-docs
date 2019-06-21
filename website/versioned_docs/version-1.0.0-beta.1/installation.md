---
id: version-1.0.0-beta.1-installation
title: Installation
sidebar_label: Installation
original_id: installation
---

The first step is including a `<script>` tag before closing of the `</head>` tag in HTML page:

```html
<html>
  <head>
    ...
    <script async src="https://bellugg-booking-widget.s3-ap-southeast-1.amazonaws.com/dist/bellugg-widget.js"></script>
  </head>
  ...
</html>
```

Then put a widget tag `<bellugg-location></bellugg-location>` in the body section:

```html
<html>
  ...
  <body>
    ...
    <bellugg-location api-key="YOUR_BELLUGG_API_KEY"></bellugg-location>
    ...
  </body>
</html>
```

### Available widget attributes
| Attribute | Value  | Description                                      |
| --------- | ------ | ------------------------------------------------ |
| api-key   | string | Your Bellugg API key                             |
| color     | string | HEX color code for widget form<br>e.g. `#990000` |