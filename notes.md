# Fixeando Prettier en este proyecto

**Para configurar Prettier correctamente y que formatee archivos Tailwind y Astro sin problemas, tome los siguientes pasos:**

## 1) Instale las siguientes Devs Dependencies:

npm install --save-dev prettier prettier-plugin-tailwindcss
npm install --save-dev prettier prettier-plugin-astro

## 2) Cree el archivo .prettierignore con la siguiente config:

node_modules
tailwind.config.mjs

## 3) Cree el archivo .prettierrc con la siguiente config:

{
"plugins": ["prettier-plugin-astro"],
"overrides": [
{
"files": "*.astro",
"options": {
"parser": "astro"
}
}
]
}

**Luego de realizar todos estos, Prettier funciono como de costumbre**

# Clases de Tailwind:

La clase "w" y "h", en vez de poner individualmente sus valores, si el valor es el mimso, se puede utilizar la etiqueta "size" para lograr el mismo efecto con solo 1 etiqueta

**Ejemplo:** "w-6 h-6" ===> "size-6"

# Dato curioso

**Por algun motivo, el icono de Astro.astro no se puede renderizar a menos que se llame distinto, en el proyecto cambie Astro.astro por Astre.astro y me lo permitio renderizar con un map**
