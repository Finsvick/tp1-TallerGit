# Ramas

Una rama es una línea de trabajo aparte. Te deja hacer cambios sin tocar `main` hasta que estén listos.

## Ver las ramas

```bash
git branch
```

La que estás usando aparece con un asterisco.

## Crear una rama

```bash
git branch docs-ejemplo
```

Crea la rama pero no te mueve a ella.

## Cambiar de rama

```bash
git switch docs-ejemplo
```

## Crear y cambiar de una

```bash
git switch -c docs-ejemplo
```

## Juntar ramas

Para traer los cambios de una rama a `main`, primero te parás en `main` y después hacés el merge.

```bash
git switch main
git merge docs-ejemplo
```

Si las dos ramas cambiaron la misma línea, Git avisa que hay un conflicto y lo tenés que resolver a mano antes de seguir.

## Borrar una rama

```bash
git branch -d docs-ejemplo
```

Solo la borra si ya se juntó con otra rama.
