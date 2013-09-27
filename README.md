TYPO3 Neos Flexslider Plugin
============================

This is a TYPO3 Neos plugin that adds very basic support for WooThemes' Flexslider to your site.

Installation
------------
1. Require the package using composer
```
composer require timkandel/flexslider:dev-master
```

2. Include the packages TypoScript in your sites'
```
include: resource://TimKandel.Flexslider/Private/TypoScripts/Library/NodeTypes.ts2
```

3. Add both the css and the JS to your template
```
<link rel="stylesheet" href="{f:uri.resource(path:'Styles/flexslider.css', package: 'TimKandel.Flexslider')}" media="all" />
```

```
<script src="{f:uri.resource(path:'JavaScript/jquery.flexslider-min.js', package: 'TimKandel.Flexslider')}"></script>
```

NOTE: Flexslider requires jQuery to work. If you don't use it on your site, you can do so by adding the following line to your template:
```
<script src="http://code.jquery.com/jquery-1.10.1.min.js"></script>
```