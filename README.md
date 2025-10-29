# Zephyr POC

The command from the [Docs](https://docs.zephyr-cloud.io/tutorials/metro) ask to run:

```bash
npm add --dev zephyr-metro-plugin @module-federation/metro @module-federation/metro-plugin-rnc-cli @module-federation/runtime
```

But I had the following error:

```bash
npm error notarget No matching version found for zephyr-rollx-internal@0.0.56.
```

The solution was to run passing version @1.0.0 to zephyr-metro-plugin:

```bash
% npm add --save-dev zephyr-metro-plugin@1.0.0
 @module-federation/metro @module-federation/metro-plugin-rnc-cli @module-federation/ru
ntime
npm warn deprecated zephyr-metro-plugin@1.0.0: Published prematurely, use latest instead

added 65 packages, changed 13 packages, and audited 978 packages in 9s

179 packages are looking for funding
  run `npm fund` for details

found 0 vulnerabilities
```