# Add-to-cart-info

Componente que realiza la función de mostrar la infromación del producto una vez se agrega el producto al carrito.

![Preview](../assets/image__add-to-cart-info.png)

## Configuration 

### Paso 1 - Clonar

Para empezar, [clonar](https://github.com/LauraCastellanos13/itgloberspartnercl-add-to-cart-info) este reopositorio para iniciar con la configuración básica. 
### Paso 2 - Editar 'manifest.json'

Una vez abierto el repositorio de manera local, ingresar al archivo `manifest.json` y allí es donde realizará modificaciones en los siguientes elementos: `vendor`, `name`, `version`, `title` y `description`. Como en el siguiente ejemplo:

```
{
 "vendor": "itgloberspartnercl",
  "name": "add-to-cart-info",
  "version": "0.0.1",
  "title": "Add to cart info",
  "description": "This component will display additional information when adding to the shopping list",
}
```

### Paso 3 - Revisar builders y dependencias

Una vez modificada esa sección del `manifest.json`, se debe rectificar que el repositorio contenga los builders y dependencias necesarios:

```
  "builders": {
    "react": "3.x",
    "messages": "1.x",
    "docs": "0.x",
    "store": "0.x"
  },
  "dependencies": {
    "vtex.checkout-resources": "0.x",
    "vtex.order-manager": "0.x",
    "vtex.product-context": "0.x"
  }
```

### Paso 4 - Instalar node-modules

Se debe ubicar en la carpeta `react`, por medio de cd.. en la terminal local o desde la carpeta del proyecto, abriendo una terminal. Una vez allí, ingresar el comando: `yarn install` y se llevará adelante una instalación de las dependencias necesarias.

### Paso 5 - Ejecute un preview 

Finalmente, después de seguir los pasos anteriores, podremos ver los cambios que se han realizado, de manera local, en el entorno o workspace que se está usando. 
Para esto, debe ingresar, en su terminal, el comando: `vtex link`, donde si todo corre bien, verá el mensaje: `App linked successfully` y su componente custom estará en orden para usar. 
Si por el contrario, en su consola sale un error, lo que deberá hacer, será recitifcar los pasos anteriormente mencionados.

### Paso 6 - Usar componente custom en la página

Para agregar este componente custom, deberá ingresar en su proyecto, ir al archivo `manifest.json` y en `dependencies`, importar el: vendor, name y versión de este repositorio. Por ejemplo:

```
  "dependencies": {
    "itgloberspartnercl.add-to-cart-info": "0.x"
  }
```
## Contributors
1. Laura Castellanos


