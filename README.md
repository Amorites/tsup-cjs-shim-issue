## repro of https://github.com/egoist/tsup/issues/485

"And somehow cjs_shim.js is introduced in cjs build (still I haven't figured out why)"

```
pnpm install
cd packages/a
pnpm build
```

packages/a/dist/index.js has an unused `importMetaUrlShim`
