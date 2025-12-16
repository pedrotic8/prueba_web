# Mini proyecto Git

## Autor
Iván

## Descripción del proyecto
Este repositorio corresponde a un mini proyecto de práctica con Git cuyo objetivo es aprender a crear la estructura inicial de un proyecto, trabajar con Git desde la terminal (Git Bash), gestionar ramas (feature y hotfix), realizar commits y organizar un proyecto con parte Java y parte web.

El proyecto está dividido en dos partes principales:
- src → código Java
- web → archivos HTML y CSS

---

## Estructura del proyecto

mini-proyecto-git/
│
├── README.md
├── .gitignore
├── src/
│ └── Main.java
└── web/
├── index.html
└── styles.css
---

## Pasos realizados

### 1. Acceso al directorio de trabajo

```bash
cd Documents/
cd prueba_web
mkdir mini-proyecto-git
cd mini-proyecto-git
touch README.md
mkdir src
cd src
touch Main.java
cd ..
mkdir web
cd web
touch index.html
touch styles.css
cd ..
touch .gitignore
git add .
git commit -m "Commit inicial donde hemos creado la estructura inicial del proyecto"
git log --oneline
git branch feature-java-utils
git branch feature-web-layout
git branch hotfix-readme
git checkout feature-java-utils
nano src/Main.java
git add src/Main.java
git commit -m "Añado a la rama java-utils la carpeta src y el main.java"
git checkout master
git branch -d feature-java-utils
git branch -d feature-web-layout
git branch -d hotfix-readme
cd src
git branch feature-java-utils
git checkout feature-java-utils
nano Main.java
git add .
git commit -m "Añado a la rama java-utils la carpeta src y el main.java"
git branch feature-web-layout
git checkout feature-web-layout
cd web
git checkout -b feature-web--layout
nano index.html
nano styles.css
git add .
git commit -m "Hago el commit para el html y css"
cd ..
git branch hotfix-readme
git checkout -b hotfix--readme

