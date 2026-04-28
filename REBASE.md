# Fusión de commits

Documento del proceso para fusionar el historial de commits.

## Proceso realizado

1. **Simulación de historial sucio**: Se ejecutaron 3 echo y sus respectivos commits con mensajes no descriptivos.
2. **Ejecución del comando**: Se utilizó `git rebase -i HEAD~3` para acceder al historial de los 3 últimos commits.
3. **Aplicación de Squash**: Se utilizó la instrucción `squash` (y su abreviatura `s`) en los commits 2 y3 para fusionar el código en el primer commt manteniendolo con `pick`.
4. **Unificar mensaje**: Se guardo una única descripción de commit: `refactor: limpieza del historial y fusión de 3 commits de prueba`.
5. **Sincronización**: Para sincronizar los cambios de los commits locales con el servidor, `git push`no funciona, por lo que hay que utilizar `git push --force`.

## Conclusión
Gracias a `git rebase` se mantiene el historial limpio y ordenado.
