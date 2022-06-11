# Ejemplo React con Vite y deploy en Github Pages

````
npm create vite

✔ Project name: … react-vite-example
✔ Select a framework: › react
✔ Select a variant: › react

Scaffolding project in ---/react-vite-example...

Done. Now run:

  cd react-vite-example
  npm install
  npm run dev


npm run build

npm run preview

# Despliegue en Github Pages
npm i gh-pages
```

## Despliegue en Github Pages

https://vitejs.dev/guide/static-deploy.html#github-pages

```
export default defineConfig({
  plugins: [react()],
  base: '/react-vite-example',
})
```

Crear deploy.sh

```
npm run build

npx gh-pages -d dist
```

