# Configurar el nombre de usuario y correo

con los siguientes comandos escribes en el archivo de configuracion de git.

```bash
git config --global user.name "Tu Nombre"
git config --global user.email "Tu Correo"
```

---

# Verificas la configuracion

con el siguiente comando podras ver el contenido del archivo de configuracion de tu sistema git.  

```bash
git config --list
```

Ahi debera estar tu nombre y tu correo.

# Crear el directorio del repositorio

Si aún no tienes una carpeta para tu proyecto, créala y entra en ella:

```bash
mkdir mi_repositorio  # Crea la carpeta
cd mi_repositorio  # Entra en la carpeta
```

---

# Inicializar el repositorio

Para convertir la carpeta en un repositorio de Git, usa:

```bash
git init
```

Esto creará una carpeta oculta llamada .git, donde se almacenará la configuración y el historial del repositorio.

---

# Agregar archivos al repositorio

Crea un archivo de prueba:

```bash
touch archivo.txt
```

Luego, agrega el archivo al área de preparación:

```bash
git add archivo.txt
```


---

# Confirmar (commit) los cambios

Registra los cambios en el historial del repositorio con un mensaje:

```bash
git commit -m "Primer commit: Agregando archivo de prueba"
```

---

# Verificar el estado del repositorio

```bash
git status  # Muestra los cambios pendientes y el estado del repositorio.
git log  # Muestra el historial de commits.
```