# nutts

El objetivo de este script de python, es detectar, añadir y eliminar, cualquier clave de acceso cuya inactividad supere cierto tiempo.
Añadiendo una capa de seguridad, que podríamos ampliar con más funcionalidad, refactorizando el script para usar lambda y steps sobre AWS.

La funcionalidad es simple, listar todas las claves de acceso utilizando regex para el parametro de UserName de la función list_access_keys, una vez tengamos la clave consultamos su último uso y en el caso, de que coincida con nuestra configuración, solo nos queda desactivarla. :balloon: 
