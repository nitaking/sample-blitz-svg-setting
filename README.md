Reference:  https://github.com/vercel/next.js/issues/14892
Detail commit: https://github.com/nitaking/sample-blitz-svg-setting/commit/58649f378bbce466fa43e29418c1a03260bfbb92

# How to this

👇install
```bash
yarn add babel-plugin-inline-react-svg
yarn add babel-plugin-module-resolver
```

👇edit `babel.config.js`

```diff
module.exports = {
  presets: ["next/babel"],
--  plugins: [],
++  plugins: [
++    ["module-resolver", { "root": ["."] }],
++    "inline-react-svg",
++  ],
}
```

![image](https://user-images.githubusercontent.com/10850034/93666215-46ae2b00-fab7-11ea-9492-915c2b4f3ad5.png)
