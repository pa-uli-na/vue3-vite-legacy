# Test Vite + Legacy

[Dokumentacja: @vitejs/plugin-legacy](https://github.com/search?q=%40vitejs%2Fplugin-legacy&type=code)

Branch: [Vite + Legacy + Quasar](https://github.com/pa-uli-na/vue3-vite-legacy/blob/vite_vite/plugin-legacy_quasar/README.md)

## Konfiguracja

Zainstaluj paczkę "@vitejs/plugin-legacy": "^1.7.1"

Wprowadź zmiany w vite.config.ts:

```
import legacy from "@vitejs/plugin-legacy";
...

export default defineConfig({
  plugins: [
    vue(),
    legacy({
      targets: ["ie >= 11"],
      additionalLegacyPolyfills: ["regenerator-runtime/runtime"],
    }),
  ],

});

```

# Uruchom i sprawdź

Buildujemy wersję

```
npm run build
```

Uruchamiamy zbuildowaną wersję:

```
npm run preview
```

Sprawdzamy na odpowiedniej przeglądarce
