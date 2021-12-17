# Issues


## Sass / scss
It seems that there are some issues either with Sass/scss or Tailwind. 

The node-sass should be replaced with sass: https://stackoverflow.com/questions/68095626/node-sass-with-apple-m1-big-sur-and-arm64 

# Setting up a new Nuxt project

## nuxt-tailwindcss: 
v4.1.0
5/5/2021
Update tailwind to 2.1 to natively support JIT (#326) (dfa989a)

The tailwind-css forms seem to be only supporting tailwind 2.0. So the issues might be due to us using 2.1.
https://www.npmjs.com/package/@tailwindcss/forms 

Next strategy:
- Go through existing project and test different versions start from middle.
- 
