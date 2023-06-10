## This branch illustrates the current Remix issue when using `tsx watch` directly:

![image](https://github.com/remix-run/remix/assets/84349818/d2170f89-4a72-470a-a222-883c42d27efc)

`tsx watch` seems to be looping, so the dev server never starts.

This can be worked around by editing `node_modules\@remix-run\dev\dist\devServer_unstable\index.js` line 139:

```jsx
-         stdio: "pipe",
+         stdio: ['ignore', 'inherit', 'inherit'],
```

![image](https://github.com/remix-run/remix/assets/84349818/fab31602-e52c-4fd4-ab36-ca6bd875bae9)


