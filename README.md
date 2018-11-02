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
