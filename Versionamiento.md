# Guía de Git Flow

## Introducción a Git Flow
Git Flow es una estrategia de trabajo en Git que facilita la gestión de ramas y la implementación de nuevas funcionalidades, correcciones y despliegues. 

## Principales Ramas en Git Flow
1. **master**: Contiene el código en producción.
2. **develop**: Contiene el último código desarrollado y probado.

## Ramas Auxiliares
1. **feature/**: Se utilizan para desarrollar nuevas funcionalidades. Nacen de la rama `develop` y al finalizar se fusionan de nuevo en `develop`.
2. **release/**: Preparan el código para una nueva versión. Nacen de `develop` y se fusionan en `master` y `develop` una vez finalizadas.
3. **hotfix/**: Se utilizan para corregir errores críticos en producción. Nacen de `master` y se fusionan en `master` y `develop`.

## Comandos de Git Flow

### Iniciar Git Flow
Para iniciar Git Flow en tu proyecto:
```sh
git flow init
```

## Crear una Nueva Funcionalidad
Para crear una nueva funcionalidad:
```sh
git flow feature start <nombre-feature>
```

## Finalizar una Funcionalidad
Para finalizar una funcionalidad:
```sh
git flow feature finish <nombre-feature>
```

## Crear una Nueva Versión (release)
Para crear una nueva versión:
```sh
git flow release start <nombre-release>
```

## Finalizar una Versión
Para finalizar una versión:
```sh
git flow release finish <nombre-release>
```

## Crear una Corrección Rápida (hotfix)
Para crear una corrección rápida:
```sh
git flow hotfix start <nombre-hotfix>
```

## Finalizar una Corrección Rápida
Para finalizar una corrección rápida:
```sh
git flow hotfix finish <nombre-hotfix>
```

## Beneficios de Git Flow
- Mejora la organización del código.
- Facilita la colaboración en equipos grandes.
- Ayuda a mantener el control de versiones y la estabilidad del código en producción.

## Recursos Adicionales
Para más detalles sobre la implementación y uso de Git Flow, consulta los siguientes recursos:

GFourmis: GitFlow: ¿Qué es y cómo aplicarlo?
https://gfourmis.co/gitflow-sin-morir-en-el-intento/

Desarrollowp: Aprende Git de manera sencilla
DEV Community: Git-Flow: Lo Esencial
