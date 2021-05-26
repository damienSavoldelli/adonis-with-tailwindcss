# adonis-with-tailwindcss
Install tailwindcss with adonisJS 5

1. Install tailwindcss, postCss & autoprefixer
```
npm install -D tailwindcss@latest postcss@latest autoprefixer@latest
```

2. Initialize tailwindcss config file
```
npx tailwindcss init
```

3. Create postcss.config.js file, with configs
```javascript
const tailwindcss = require('tailwindcss')
const autoprefixer = require('autoprefixer')

module.exports = {
  plugins: [
    tailwindcss,
    autoprefixer,
  ]
}
```

4. Enable support postCSS in webpack config
```javascript
Encore.enablePostCssLoader()
```

5. Install postcss-loader 
```
npm install -D postcss-loader
```

6. execute adonis serve to compile (in watch mode)
```
node ace serve -w
```


7. Tailwindcs is installed & compil in apps.css, Let's working !
![app.css](docs/screenshots/screen-app.css.png)



Source :
- adonisJS doc : 
  - [activate postCss](https://docs.adonisjs.com/guides/assets-manager#setup-postcss)

- Tailwindcs doc:
  - [Install tailwindcss](https://tailwindcss.com/docs/installation)
  - [Congfiguration](https://tailwindcss.com/docs/configuration)
  - [JIT](https://tailwindcss.com/docs/just-in-time-mode)

- PostCss:
  - [Site](https://postcss.org/)
  - [Github repo](https://github.com/postcss/postcss)
  - [plugins list](https://www.postcss.parts/)

- videos :
  - [RomanLanz Twicth explain how to install & config tailwind css](https://www.twitch.tv/videos/1024929427) (possible 404)
  - [Explain postCss from grafikrat (fr)](https://grafikart.fr/tutoriels/postcss-663)

