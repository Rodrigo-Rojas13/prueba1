# Comandos de Git y GitHub

Una guía completa de los comandos más utilizados en Git y GitHub.

---

## 🛠️ Configuración Inicial

| Comando | Descripción | Ejemplo |
|--------|-------------|---------|
| `git config --global user.name "Tu Nombre"` | Configura el nombre de usuario global | `git config --global user.name "Juan Pérez"` |
| `git config --global user.email "email@example.com"` | Configura el correo electrónico global | `git config --global user.email "juan@example.com"` |
| `git config --global core.editor nano` | Define el editor por defecto | `git config --global core.editor "code --wait"` |

---

## 📁 Crear o Clonar Repositorios

| Comando | Descripción | Ejemplo |
|--------|-------------|---------|
| `git init` | Inicializa un nuevo repositorio local | `git init` |
| `git clone <url>` | Clona un repositorio remoto | `git clone https://github.com/user/proyecto.git` |

---

## 📄 Seguimiento de Archivos

| Comando | Descripción | Ejemplo |
|--------|-------------|---------|
| `git status` | Muestra el estado del repositorio | `git status` |
| `git add <archivo>` | Añade archivos al área de preparación (staging) | `git add index.html` |
| `git add .` | Añade todos los archivos modificados | `git add .` |
| `git reset <archivo>` | Quita un archivo del área de preparación | `git reset index.html` |

---

## 📦 Commits

| Comando | Descripción | Ejemplo |
|--------|-------------|---------|
| `git commit -m "mensaje"` | Crea un commit con un mensaje | `git commit -m "Agrega login"` |
| `git commit -am "mensaje"` | Añade y comitea archivos ya trackeados | `git commit -am "Corrige errores"` |
| `git commit --amend` | Modifica el último commit | `git commit --amend -m "Nuevo mensaje"` |

---

## 🔁 Ramas

| Comando | Descripción | Ejemplo |
|--------|-------------|---------|
| `git branch` | Lista ramas locales | `git branch` |
| `git branch <rama>` | Crea una nueva rama | `git branch feature-login` |
| `git checkout <rama>` | Cambia de rama | `git checkout main` |
| `git checkout -b <rama>` | Crea y cambia a una nueva rama | `git checkout -b feature-home` |
| `git merge <rama>` | Une una rama con la actual | `git merge develop` |
| `git branch -d <rama>` | Elimina una rama local | `git branch -d old-branch` |

---

## 📤 Sincronización Remota

| Comando | Descripción | Ejemplo |
|--------|-------------|---------|
| `git remote -v` | Lista las URLs remotas | `git remote -v` |
| `git remote add origin <url>` | Agrega un repositorio remoto | `git remote add origin https://github.com/user/repo.git` |
| `git push` | Envía los commits al remoto | `git push origin main` |
| `git pull` | Trae los cambios del remoto | `git pull origin main` |
| `git fetch` | Descarga cambios pero no los mezcla | `git fetch origin` |

---

## 🪄 Otros Comandos Útiles

| Comando | Descripción | Ejemplo |
|--------|-------------|---------|
| `git log` | Muestra el historial de commits | `git log` |
| `git diff` | Muestra diferencias entre archivos | `git diff` |
| `git stash` | Guarda cambios sin commitear temporalmente | `git stash` |
| `git stash apply` | Recupera los cambios del stash | `git stash apply` |
| `git tag <nombre>` | Crea un tag | `git tag v1.0.0` |

---

## 💣 Deshacer Cambios

| Comando | Descripción | Ejemplo |
|--------|-------------|---------|
| `git checkout -- <archivo>` | Descarta cambios en un archivo | `git checkout -- index.html` |
| `git revert <hash>` | Revierte un commit específico | `git revert a1b2c3` |
| `git reset --hard HEAD` | Revierte todo al último commit | `git reset --hard HEAD` |

---

## 🔄 Reescritura de Historial (⚠️ Avanzado)

| Comando | Descripción | Ejemplo |
|--------|-------------|---------|
| `git rebase <rama>` | Reescribe la base de una rama | `git rebase main` |
| `git cherry-pick <hash>` | Aplica un commit específico a la rama actual | `git cherry-pick a1b2c3` |

---

## 🌐 GitHub CLI (Opcional)

| Comando | Descripción | Ejemplo |
|--------|-------------|---------|
| `gh auth login` | Inicia sesión en GitHub desde la terminal | `gh auth login` |
| `gh repo create` | Crea un nuevo repositorio en GitHub | `gh repo create my-repo` |
| `gh issue create` | Crea una nueva issue | `gh issue create --title "Bug" --body "Descripción"` |
| `gh pr create` | Crea un pull request | `gh pr create --base main --head feature-1` |

---

## 📌 Buenas Prácticas

- Usar mensajes de commit claros y concisos
- Hacer `pull` antes de hacer `push`
- Crear ramas para nuevas funcionalidades
- Usar `.gitignore` para excluir archivos innecesarios
- Revisar el historial antes de hacer un `push`

---

## 📚 Recursos

- [Git - Sitio oficial](https://git-scm.com/)
- [GitHub Docs](https://docs.github.com/)
- [Git Cheatsheet](https://education.github.com/git-cheat-sheet-education.pdf)

