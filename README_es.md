# Aprende Git
Aquí encontrarás un repositorio de muestra para mi serie de tutoriales en YouTube sobre cómo aprender Git y GitHub.
Si te ha resultado útil este repositorio, por favor considera darle una estrella ⭐, ya que esto hará que otros lo encuentren más fácilmente.

Además, me ayudaría mucho si te suscribes a mi [canal de YouTube](https://www.youtube.com/@richardcallaby), ya que allí publico tutoriales gratuitos y otros recursos educativos gratuitos.

## Aquí tienes un tutorial paso a paso sobre cómo contribuir en GitHub
Crea una cuenta en GitHub: Si aún no tienes una cuenta de GitHub, necesitarás crear una. Ve a github.com y haz clic en el botón "Sign up" en la esquina superior derecha. Sigue las instrucciones para crear tu cuenta.

Encuentra un repositorio al que contribuir: Una vez que tengas una cuenta en GitHub, puedes buscar repositorios que te interesen para contribuir. Usa la barra de búsqueda de GitHub para buscar repositorios por nombre o palabra clave.

Haz un fork del repositorio: Una vez que encuentres un repositorio al que quieras contribuir, necesitarás hacer un fork.

El fork crea una copia del repositorio en tu propia cuenta de GitHub, que puedes modificar sin afectar al repositorio original.

### Imagen de referencia
Haz clic en el botón de abajo para hacer un fork del repositorio que se encuentra en la esquina superior derecha.

![imagen_fork](./images/Readme_images/fork.png)

Clona el repositorio forkeado: Después de hacer un fork del repositorio, necesitarás clonarlo en tu máquina local. Clonar crea una copia del repositorio en tu computadora con la que puedes trabajar. Para clonar el repositorio, abre una ventana de terminal e introduce el siguiente comando:

```
git clone https://github.com/tu-usuario/nombre-del-repositorio.git
```

Asegúrate de reemplazar "tu-usuario" y "nombre-del-repositorio" con tu nombre de usuario de GitHub y el nombre del repositorio que forkeaste.

### Imagen de referencia
![clonar_repo](./images/Readme_images/Clone.png)

Asegúrate de crear una rama con un nombre único para reflejar los cambios que deseas hacer en el código fuente. Para crear una rama, usa la siguiente sintaxis:

```
git branch "nombre-de-la-rama"
```
### Imagen de referencia
![creacion_rama](./images/Readme_images/Branch_making.png)

Para cambiar a esa rama, usa la siguiente sintaxis:
```
git checkout "nombre-de-la-rama"
```

### Imagen de referencia
![cambio_rama](./images/Readme_images/branch_switch.png)

Haz cambios en el código: Una vez que tengas el repositorio clonado en tu máquina local, puedes hacer cambios en el código. Usa tu editor de texto o IDE preferido para modificar los archivos.

Confirma los cambios: Después de hacer cambios en el código, necesitarás confirmarlos en tu repositorio local. Para hacerlo, abre una ventana de terminal y navega a la raíz del repositorio clonado. Usa el siguiente comando para preparar los cambios:

```
git add .
```

### Imagen de referencia
![añadir](./images/Readme_images/add.png)

Esto preparará todos los cambios hechos en los archivos del repositorio.

Luego, confirma los cambios usando el siguiente comando:

```
git commit -m "Una breve descripción de los cambios realizados"
```

### Imagen de referencia
![Commit](./images/Readme_images/commit.png)

Asegúrate de incluir un mensaje breve e informativo que describa los cambios que realizaste.

Sube los cambios a GitHub: Después de confirmar los cambios en tu repositorio local, necesitarás subirlos a GitHub. Esto actualizará la copia del repositorio en tu cuenta de GitHub con los cambios que realizaste. Para subir los cambios, usa el siguiente comando:

```
git push origin nombre-de-la-rama
```

### Imagen de referencia
![Subir_imagen](./images/Readme_images/push.png)

Crea una solicitud de extracción: Después de subir los cambios a GitHub, cuando recargues el repositorio forkeado, verás la opción de crear una solicitud de extracción. Haz clic en ese botón para crear la solicitud.

### Imagen de referencia 
![Solicitud_extraccion](./images/Readme_images/pull%20request.png)

Esto te llevará a una página donde puedes revisar los cambios que realizaste y proporcionar una descripción de tu solicitud de extracción.

Asegúrate de incluir una descripción clara y concisa de los cambios que realizaste y por qué los hiciste.

Si hay algún problema o inquietud que el propietario del repositorio deba conocer, asegúrate de mencionarlo en la descripción de la solicitud de extracción.

Una vez que estés satisfecho con la descripción, haz clic en el botón "Create pull request".

### Imagen de referencia
![Crear_solicitud](./images/Readme_images/Create_pull_request.png)

Espera comentarios: Después de crear la solicitud de extracción, el propietario del repositorio revisará tus cambios y te proporcionará comentarios.

Es posible que te pidan realizar cambios adicionales, o que fusionen tus cambios en el repositorio original.

Sé paciente y receptivo durante este proceso, y asegúrate de abordar cualquier comentario o inquietud que el propietario del repositorio plantee.

Actualiza tu repositorio forkeado: Si el propietario del repositorio fusiona tus cambios en el repositorio original, necesitarás actualizar tu repositorio forkeado para reflejar esos cambios.

Para hacerlo, navega a tu repositorio forkeado en GitHub y haz clic en el botón "Fetch upstream".

Luego, ejecuta el siguiente comando en tu repositorio local para actualizarlo:

```
git pull
```

Eso debería darte una idea básica de cómo usar Git, por supuesto, puedes revisar las lecciones que he creado en este repositorio para obtener explicaciones más detalladas.

## Buen primer problema

Puedes usar este proyecto como una forma de empezar a contribuir a proyectos de código abierto. Este podría ser un **buen primer problema**, solo modifica el archivo [CONTRIBUTORS.md](https://github.com/rcallaby/Learn-Git/blob/main/CONTRIBUTORS.md) para que enlace a tu propio repositorio de GitHub. Usa markdown como se muestra en el archivo.

Por favor revisa el directorio [First-Contributions](https://github.com/rcallaby/Learn-Git/tree/main/First-Contributions) para obtener instrucciones paso a paso sobre cómo contribuir a este repositorio.

### Tabla de contenidos

- [Parte 00 - Historia y Fundación](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-00-History-and-Foundations/history-of-git.md)
- [Parte 01 - Navegación Básica](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-01-Basic-Navigation/basic-navigation.md)
- [Parte 02 - Inicializando Git](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-02-Initializing-Git/getting-started.md)
- [Parte 03 - Ramas y Fusiones](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-03-Branching-and-Merging/branching-and-merging.md)
- [Parte 04 - Colaborando con Repositorios Remotos](https://github.com/rcallaby/Learn-Git/tree/main/Lessons/en/Part-04-Collaborating-with-Remote-Repositories/collaborating-with-remote-repos.md)
- [Parte 05 - Conceptos Avanzados de Git](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-05-Advanced-Git-Concepts/advanced-git.md)
- [Parte 06 - CI-CD con Git y GitHub](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-06-CI-CD-with-Git-and-Github/ci-cd-git-github.md)
- [Parte 07 - Mejores Prácticas y Consejos para Git](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-07-Git-Best-Practices-and-Tips/best-practices-tips.md)
- [Parte 08 - Git y GitHub en el Desarrollo Ágil](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-08-Git-and-Github-in-Agile-Development/git-github-agile-dev.md)
- [Parte 09 - GitHub y Codespaces](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-09-Github-and-Codespaces/github-codespaces.md)
- [Parte 10 - Acciones de GitHub](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-10-Github-Actions/github-actions.md)
- [Parte 11 - Acciones Avanzadas de GitHub](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-11-Advanced-Github-Actions/advanced-github-actions.md)
- [Parte 12 - Usando Jupyter Codespaces en GitHub](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-12-Using-Jupyter-Codespaces-in-Github/github-jupyter-codespace.md)
- [Parte 13 - Usando C# Codespaces en GitHub](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-13-Using%20Csharp-Codespaces-in-Github/github-Csharp-codespace.md)
- [Parte 14 - Usando React Codespaces en GitHub](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-14-Using-React-Codespaces-in-Github/github-react-codespace.md)
- [Parte 15 - Usando Express Codespaces en GitHub](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-15-Using-Express-Codespaces-in-Github/github-express-codespace.md)
- [Parte 16 - Usando Ruby on Rails Codespaces](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-16-Using-Ruby-on-Rails-Codespaces/github-rubyrails-codespace.md)
- [Parte 17 - Usando Django Codespaces en GitHub](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-17-Using%20Django%20Codespaces-in-Github/github-django-codespace.md)
- [Parte 18 - Herramientas de Gestión de Proyectos de GitHub](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-18-Github-Project-Management-Tools/github-project-management-tools.md)
- [Parte 19 - Tableros de Proyectos y Notas en GitHub](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-19-Github-Project-Boards-and-Notes/github-project-boards-and-notes.md)

#### Traducciones de este tutorial
Puedes encontrar traducciones de este tutorial en varios idiomas a continuación. Ten en cuenta que algunas de estas traducciones están en progreso y no se han completado totalmente aún.

Chino (Simplificado)  
Francés  
Alemán  
Ruso  
Español  
Hindi  
Italiano  
Mongol  
Japonés
