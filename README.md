# No known conditions for "./action" specifier in "svelte" package [plugin vite:dep-scan]

run `pnpm dev` to see the error:

```
✘ [ERROR] No known conditions for "./action" specifier in "svelte" package [plugin vite:dep-scan]

script:/frontend/apps/kvist/src/ui/components/KvistPopover/KvistPopover.svelte?id=0:70:7:
  70 │ import 'svelte/action'
	 ╵        ~~~~~~~~~~~~~~~

This error came from the "onResolve" callback registered here:

../../node_modules/.pnpm/esbuild@0.24.2/node_modules/esbuild/lib/main.js:1150:20:
  1150 │       let promise = setup({
	   ╵                     ^

at setup (file:///frontend/node_modules/.pnpm/vite@6.1.0_@types+node@22.13.1_jiti@2.4.2_terser@5.37.0_tsx@4.19.2_yaml@2.7.0/node_modules/vite/dist/node/chunks/dep-CfG9u7Cn.js:18418:13)
at handlePlugins (/frontend/node_modules/.pnpm/esbuild@0.24.2/node_modules/esbuild/lib/main.js:1150:21)
at buildOrContextImpl (/frontend/node_modules/.pnpm/esbuild@0.24.2/node_modules/esbuild/lib/main.js:873:5)
at Object.buildOrContext (/frontend/node_modules/.pnpm/esbuild@0.24.2/node_modules/esbuild/lib/main.js:699:5)
at /frontend/node_modules/.pnpm/esbuild@0.24.2/node_modules/esbuild/lib/main.js:2038:68
at new Promise (<anonymous>)
at Object.context (/frontend/node_modules/.pnpm/esbuild@0.24.2/node_modules/esbuild/lib/main.js:2038:27)
at Object.context (/frontend/node_modules/.pnpm/esbuild@0.24.2/node_modules/esbuild/lib/main.js:1880:58)
at prepareEsbuildScanner (file:///frontend/node_modules/.pnpm/vite@6.1.0_@types+node@22.13.1_jiti@2.4.2_terser@5.37.0_tsx@4.19.2_yaml@2.7.0/node_modules/vite/dist/node/chunks/dep-CfG9u7Cn.js:18206:24)
```
