
# Загрузка проекта VS Code на репозиторий

**Гит игнор:**
Проекты на React (особенно с TypeScript) могут содержать большое количество файлов и занимать много места, если не настроить .gitignore должным образом. Многие из этих файлов являются промежуточными или генерируемыми автоматически, и их не нужно включать в репозиторий. Вот как можно поступить:

Создайте .gitignore
.gitignore — это файл, который указывает Git игнорировать определённые файлы и папки. Для проекта Tauri + React + TypeScript можно использовать следующий шаблон .gitignore:

```gitignore
# Node.js
node_modules/
npm-debug.log*
yarn-debug.log*
yarn-error.log*

# Build directories
/dist/
/build/
/out/
/target/

# Environment variables
.env
.env.local
.env.*.local

# IDEs and editors
.vscode/
.idea/
*.sublime-project
*.sublime-workspace

# OS generated files
.DS_Store
Thumbs.db

# Tauri specific
/src-tauri/target/
/src-tauri/.cache/
/src-tauri/Cargo.lock

# React App build artifacts
/public/build/
/public/assets/ 

```


# Стандартная гит загрузка
git add .
git commit -m "***"
git push origin main


# Скачивание с гитхаба
git clone 

# УСТАНОВКА NPM
Если таури проект скачан из гитхаба в папку, то нужно отдельно npm устанавливать
- npm install

# Дополнительно
добавить .env если нужно 
