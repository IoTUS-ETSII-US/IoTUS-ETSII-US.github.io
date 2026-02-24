![Logo Hugo](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQmG0sTTujYLYv0fIIepY8CGiS6fY6rlvNlTA&s)

# Instalar Hugo

### Linux:

```bash
sudo snap install hugo
```

[Más información / otras opciones](https://gohugo.io/installation/linux/#package-managers)

### Windows:

```bash
winget install Hugo.Hugo.Extended
```

[Más información / otras opciones](https://gohugo.io/installation/windows/#package-managers)

### MacOS:

```bash
brew install hugo
```

[Más información / otras opciones](https://gohugo.io/installation/macos/#package-managers)

# Explicación de la estructura del proyecto

- **/archetypes**: esquemas que debe seguir el contenido.
- **/content**: contenido en .md que va a renderizar la web.
- **/themes**: tema instalado que sirve como esqueleto.

**/public** y **/resources** lo genera automaticamente hugo al hacer `hugo server`

[Más información](https://gohugo.io/getting-started/directory-structure/)

# Descargar carpeta del tema

Si la carpeta del tema `/themes/papermod` aparece vacía:

```bash
git submodule update --init --recursive
```

# Iniciar el proyecto

```bash
hugo server [Flag]
```

| Flag | Descripción                                                  |
| ---- | ------------------------------------------------------------ |
| - D  | Renderiza el contenido en borrador tambien (**draft: true**) |

Para abrir la web, pinchar en el enlace `http://IP:PORT` que aparece en la teminal. Por defecto `http://localhost:1313`
