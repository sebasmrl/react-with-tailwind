# React + TypeScript + Vite

## Instrucciones para trabajar con tailwind
1. Ejecutar para instalar 
``` 
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
```

2.  Crea el archivo de configuracion en la carpeta `./src` del proyecto llamada tailwind.config.js

```js
/** @type {import('tailwindcss').Config} */
export default {
  content: [
    "./index.html",
    "./src/**/*.{js,ts,jsx,tsx}",
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

3. Anadir las siguiente propiedad para que la directiva @tailwind sea admitido en archivos css
```json
"files.associations": {
  "*.css": "tailwindcss"
}
```