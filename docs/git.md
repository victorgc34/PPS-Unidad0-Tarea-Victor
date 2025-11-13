# Creación del repositorio de Github

Para empezar con la realización de este proyecto, debemos de tener instalado instalado **Git** en nuestro equipo. Además, deberemos de registrarnos con nuestra cuenta ya sea con el comando `gh auth login` o ha través de tokens. Todo el proceso de creación del repositorio lo realizaremos a través de la terminal, por lo que no necesitaremos acceder desde la web.

Lo que realizaremos en este apartado será lo siguiente:

1. **Creación de la estructura del repositorio**
2. **Inicialización del repositorio local**
3. **Creación del repositorio en Github**

## 1.0 Creación de la estructura del repositorio

Lo primero que haremos sería definir la estructura que tendrá nuestro proyecto. Para ello, crearemos un conjunto de archivo y carpetas que nos será útiles en los próximos apartados.

La estructura que tendrá este proyecto será la siguiente:

- **docs**
    - img
        - imagenes.jpg
    - index.md
    - git.md (Donde esta escrito este apartado)
    - gitActions.md
    - docker.md
    - conclusiones.md
- **.github**
    - **workflows**
        - CreacionDocumentacion.yml
- mkdocs.yml
- README.md
- requiriments.txt

imagen tree -a

## 2.0 Inicialización del repositorio local

Lo que haremos será inicial el repositorio en la raiz de nuestra carpeta del proyecto. El comando que utilizaremos será el siguiente:

```bash
git init
```

Imange init

### 2.1 Añadimos todos los archivos

En este paso, añadiremos todos los archivos de nuestro repositorio para que en nuestro primer commint, se suban al repositorio.

```bash
git add .
```

Imange git add

### 2.2 Creación de la primera “instantánea” de nuestro repositorio

Para crear nuestro primer commint, tendremos utilizar este comando, en el cual indicaremos el motivo de este.

```bash
git commit -am "Inicio del repositorio"
```

Imagen del commint

## 3.0 Creación del repositorio en Github

Aquí, crearemos el nuestro repositorio en la nube y lo vincula con el repositorio local previamente creado. Para ello, tendremos que indicar nuestro “***nombre de usuario de github”***  y ***“Nombre del repositorio a crear”***. Además, antes de crearlo, le indicaremos la rama a la que apuntamos.

```bash
git branch -M main
gh repo create nombre-usuario/nombre-repositorio --public --source=. --remote=origin --push
```

Imange repo create

Con todo esto, ya tenemos nuestro repositorio creado y lista para trabajar en el.
