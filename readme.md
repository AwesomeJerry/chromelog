# chromelog
### Because sometimes, all you need is a `console.log` in chrome.

## We follow `breaking.feature.fix` versioning

This project came out of the frustrations faced when developing on [react-native](https://facebook.github.io/react-native/), and trying to "debug in chrome", just because I needed the good old `console.log` inside chrome so I could explore objects that I want to explore.

(for those who are not aware, __react-native's "debug in chrome"__ gives you the full fledged chrome debugger for react-native, but __makes your app crawl__, and __makes you cry__)

### Usage:
`npm install --save chromelog`

And add `"chromelog": "chromelog"` under the `"scripts"` key in your project's `package.json`. It should look something like this:

```json
{
  "name": "AwesomeReactNativeAppOrSomeOtherProject",
  "version": "0.9.0",
  "description": "Log stuff from anywhere into chrome",
  "main": "index.js",
  "scripts": {
    ...
    "chromelog": "chromelog"
  },
  ...
}
```

Now you can start the chromelog server by running this command from your project root: `npm run chromelog`

You can also install `chromelog` globally, but you do need to install it in the project where you plan to use it, so just skip the global install I'd say. With node, never install anything globally.
