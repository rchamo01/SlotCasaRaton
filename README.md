# Destellos del Universo

Página web oficial del proyecto *Destellos del Universo*, creada y publicada en 2022.

## Acceso a la web:
Existen una URL de acceso a la web online:
- URL de Github Pages: https://cslab-upm.github.io/destellosdeluniverso/

Se dispone de la URL de Github Pages que se genera automáticamente al hacer uso de Jekyll como creador de sitios web estáticos y que de acuerdo con las políticas de Github no tendrá ningún coste. Esta URL se trata de una web de proyecto que deriva de la web oficial del grupo también publicada con Github Pages en la dirección https://cslab-upm.github.io/.

## Ramas del proyecto:
El proyecto actualmente cuenta con dos ramas master y gh-pages que se describen a continuación:
- **master**: rama principal del proyecto que habrá que actualizar siempre que se haga un cambio permanente en la web.
- **gh-pages**: rama con el estado de la web que será visible. Es muy recomendable que esta rama siempre sea igual a la rama master ya que master debería tener la última versión (versión estable) del proyecto y gh-pages tendrá esta versión, que será la que se muestre.

Si se desean crear nuevas ramas de desarrollo se pueden crear con normalidad y emplear como sea necesario, pero si se desean aplicar los cambios de esta nueva rama a la rama principal, habrá que actualizar ambas ramas (master y gh-pages). En concreto, si queremos visualizar los cambios en la web tendremos que asegurarnos de que hacemos un merge con la rama gh-pages.

## Subir cambios:
**Buenas prácticas:**
Comprobar en qué rama estamos:
```
git status
```
Si queremos cambiar a master:
```
git checkout master
```
Si queremos cambiar a gh-pages:
```
git checkout gh-pages
```

Una vez estamos en la rama que queremos, nos traemos los cambios de la web antes de hacer nuevas modificaciones para evitar conflictos.
```
git pull
```

**Aplicar cambios:**
Realizamos las modificaciones y creamos un nuevo commit normalmente. Cuando se ha creado el commit y se ha hecho el push, cambiamos a la rama gh-pages o master (la que no esté actualizada), y hacemos un merge de la rama actualizada. Por ejemplo, si estamos en master:
```
git checkout gh-pages
git merge master
git push
```
