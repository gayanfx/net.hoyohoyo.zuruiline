ZuruiLine
====

Drawing smart line widget for [Titanium](http://www.appcelerator.com/platform) [Alloy](http://projects.appcelerator.com/alloy/docs/Alloy-bootstrap/index.html). This widget draw a line with high-light called ZURUI-SEN(ズルい線)[^1] in Japanese.

How to Use
----
* Download and deploy the widget under `app/widgets/net.hoyohoyo.smartline`.
* Add the widget as a dependency to your `app/config.json` file like so:

```javascript
	…
	"dependencies": {
		"net.hoyohoyo.smartline": "1.0"
	}
```

* Use the widget in a view with `Widget` tag like so:

```xml
<Widget id="line" src="net.hoyohoyo.smartline" />
```

* Set style in a tss file like so:

```javascript
'#line': {
	top: '100dp',
	width: '75%',
	alphaBlack: 0.3,
	alphaWhite: 0.7
}
```

Sample Screenshot
----
![screenshot](./screenshot.png)

Sample TSS Code
----
```javascript
'#line1': {
  top: '50dp',
  width: '75%',
  alphaBlack: 0.3,
  alphaWhite: 0.7
},
'#line2': {
  top: '100dp',
  width: '50%',
  alphaWhite: 0.9,
  gradientEnabled: false
},
'#line3': {
  top: '150dp',
  width: '80%',
  alphaBlack: 0.4,
  alphaWhite: 1,
  gradientPosition: 0.5
},
'#line4': {
  top: '200dp',
  width: '100%',
  alphaBlack: 0.1,
  alphaWhite: 0.5,
  gradientEnabled: false
},
'#line5': {
  top: '250dp',
  width: '50%',
  gradientPosition: 0.1
}
```

Available Properties
----
- alphaBlack : Number

  Alpha channel value of black (upper) line. (Range: 0 to 1)

- alphaWhite : Number

  Alpha channel value of white (lower) line. (Range: 0 to 1)

- bottom : Number/String

  Line's bottom position, in platform-specific units.

- gradientEnabled : Boolean

  Determines whether the alpha channel gradation on sides is enabled. (Default: true)

- gradientPosition : Number

  Position end of gradation on sides. (Default: 0.25, Range: 0 to 0.5)

- left : Number/String

  Line's left position, in platform-specific units.

- right : Number/String

  Line's right position, in platform-specific units.

- top : Number/String

  Line's top position, in platform-specific units.

- width : Number/String

  Line's width, in platform-specific units.


[^1]: Inspired by [@ken_c_lo](https://twitter.com/ken_c_lo)'s "Zurui Design Technique" [English version](https://speakerdeck.com/ken_c_lo/zurui-design-technique-english-version) [日本語版](https://speakerdeck.com/ken_c_lo/zurui-design) 