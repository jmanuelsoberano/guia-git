# Comandos básicos


## Configuracion inicial
```
git config --global user.name "Nombres Apellidos"
git config --global user.email "correo@dominio.com"
```

#### Verifica lo que se tiene configurado hasta el momento
```
git config --global -l
```

#### Inicializar git
```
mkdir proyecto1
cd proyecto1
git init

echo "Fichero1" > fichero1.txt
git add fichero1.txt
git commit -m "Creando fichero1.txt"
git log
git add .
git commit -m "commit todo"
```

## Areas en git
| STASH         | WORKSPAGE     | INDEX | LOCAL REPOSITORY | UPSTREAM REPOSITORY
| ------------- |:-------------:| -----:| -----:           | -----:             |
| [stash] | Zona de trabajo en donde tenemos los ficheros | Stage Area [add] | .git [commit] | [push] |
| LOCAL         | LOCAL         | LOCAL | LOCAL            | REMOTO             |

## Comandos
### git add
#### Un o varios archivos
```
git add *.c
git add index.html
```
#### Un directorio
```
git add <directorio>
```

### git commit
```
git commit –m “message”
```
#### Si el archivo se administra por el repo:
```
 git commit –am “message” 
```

### git rm
#### Antes del primer commit
```
git rm  --cached  <file>
```
#### Despues del primer commit
```
git reset HEAD <files> 
```

Workflow:

![alt text](https://sselab.de/lab2/public/wiki/sselab/images/thumb/4/4f/Git_workflow.png/800px-Git_workflow.png "Versión 1")

![alt text](https://res.cloudinary.com/fengerzh/image/upload/git-reset_drbfhd.png "Versión 2")

