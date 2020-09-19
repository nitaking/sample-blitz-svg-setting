Reference:  https://github.com/vercel/next.js/issues/14892

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
