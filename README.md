# learning-vue

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).

### Setting up formatting in VSCode

1. install Beautify
2. add this to settings.json (skip anything that's already there):

```
"editor.formatOnSave": true,
"[html]": {
	"editor.defaultFormatter": "HookyQR.beautify"
},
"vetur.format.defaultFormatter.html": "js-beautify-html",
"vetur.format.defaultFormatter.js": "none",
"vetur.format.defaultFormatterOptions": {
	"js-beautify-html": {
		"wrap_attributes": "auto"
	}
}
"editor.codeActionsOnSave": {
	"source.fixAll": true
}
```

which does the following:

i. turns on format on save

ii. sets default .html formatter to Beautify 

iii. sets vetur's html formatter to Beautify

iv. sets vetur's js formatter to none (we will use eslint for this)

v. turns off html attribute wrapping in vetur (it won't make a new line for every attribute)

vi. turns on auto-fix on save for eslint



note: i-iv can be done using the settings UI, but v and vi have to be inserted manually
