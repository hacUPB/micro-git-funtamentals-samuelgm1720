# Crear un repositorio en GitHub

1. Ve a [GitHub](https://github.com/) e inicia sesión.  
![alt text](<../images/Captura de pantalla 2025-01-31 160402.png>)
2. En la parte superior derecha, haz clic en el botón *New* (o ve a [GitHub New Repository](https://github.com/new)).  
![alt text](<../images/Captura de pantalla 2025-01-31 160509.png>)
3. Ingresa un nombre para el repositorio (por ejemplo, mi_repositorio).  
4. Haz clic en *Create repository*.  

---

# Agregar y confirmar archivos en el repositorio local

Crea un archivo y agrégalo al control de versiones:

```bash
touch archivo.txt
git add .
git commit -m "Primer commit: Archivo de prueba"
```

---

# Vincular el repositorio local con GitHub

Ahora debes conectar el repositorio local con el que creaste en GitHub:

```bash
git remote add origin https://github.com/tu_usuario/mi_repositorio.git
```

Puedes verificar que se agregó correctamente con:

```bash
git remote -v
```

---

# Subir los archivos a GitHub
modifica  el archivo en este caso `archivo.txt` y realiza un commit con los cambios.  
Despues verifica el estado.  

```bash
git status

On branch master
Your branch is ahead of 'upstream/master' by 1 commit.
(use "git push" to publish your local commits)

nothing to commit, working tree clean
```
Ahora, envía los archivos al repositorio remoto con:

```bash
git push
```

Despues de esto verifica el estado 
```bash
git status

On branch master
Your branch is up to date with 'upstream/master'.

nothing to commit, working tree clean
```


---

# Sincronizar futuros cambios

Cada vez que hagas cambios en tu repositorio local, usa estos comandos para actualizarlos en GitHub:

```bash
git add .
git commit -m "Descripción de los cambios"
git push 
```

Si quieres traer los cambios más recientes desde GitHub a tu computadora, usa:

```bash
git pull origin main
```