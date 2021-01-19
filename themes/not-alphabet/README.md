# notAlphabet Rocket Theme

This is a theme/preset for [Rocket](https://rocket.modern-web.dev/).

It is a rocket theme, inspired by the look of abc.xyz

## Installation

```
npm i -D @webappwriter/not-alphabet-rocket-theme
```

Add it to your 👉 `rocket.config.js`, perhaps like so, assuming you are also using rocketLaunch(). 

The order is important. rocketLaunch() would need to come first.

```js
import { rocketLaunch } from '@rocket/launch';
import { notAlphabetTheme } from '@webappwriter/not-alphabet-rocket-theme';

export default {
  presets: [rocketLaunch(), notAlphabetTheme()],
};
```