
# Resumen de comandos GIT

A Little manual on how to use git

## crear un repo local

please, run the following command

```bash
  git status
  git init NombredeRepoLocal
  git branch -a
```
## clonar un repo remoto

En el github ubicar o crar el repo remoto, para que luego sea clonado localmente

```bash
  git clone https://github.com/usuarioGit/Nombrerepo.git
  
```
Luego accdeder al directorio de trabajo

```bash
  cd Nombrerepo
  ls
  git remote -v  
```

### Agregar cambios:
```bash
  git status
  git add . 
```

para guardar en el repositorio local debemos hacer un commit:

```bash
  git commit -m "este es mi primer commit" 
```

### Guardar cambios en repositorio remoto (github):
antes de guardar los cambios hay que darse de alta en la pc con tu email y user:

```bash
	git config --local user.email steampunkkraken@cephalopod.com
	git config --local user.name deepcoder
```
luego subir al repositorio remoto:

```bash
  git remote -v
  git push origin main 
```
Al hacer esto te solicitará tu usuario hithub y cuando solicite el password colocas el tokeken gitgub (previamente hay que generar un token)

```bash
  El token es algo asi:
  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
```

### Crear una Rama:
crear una ram llamada dev:
```bash
  git checkout -b dev
```

### ver todas las ramas locales y remotas:
(-a = all)
```bash
  git branch -a
```
### Cambiar de Branch o rama:
(-a = all)
```bash
  git checkout nameofBranch
  ejemplo:
  git checkout main
  git checkout dev
```