# Apéndice — Aportaciones técnicas concretas

Resumen: Material de respaldo, no contenido principal de slides. Citado desde **5.4** como evidencia de que el equipo cubre función de arquitectura más allá del oficio nominal — eso es parte de por qué el departamento de arquitectura del cliente W2M tiene buen concepto del equipo y por qué el diseño de la intranet (5.3) tiene legitimidad operativa.

## Springpack para Excels masivos

La solución completa requirió **cambiar el recolector de basura de la JVM** y **reorganizar la memoria del contenedor** (split entre servidor — Apache o Netty — y aplicación). Si das de más memoria a la app, ésta la usa, y si no está bien repartido, la app puede comerse al servidor en runtime.

## Grafos cíclicos en BBDD W2M

Hoteles con **múltiples IDs en distintas plataformas** (datos no actualizados consistentemente) producían **bucles infinitos** al recorrerse el grafo. Resuelto con **algoritmos específicos**. El departamento de arquitectura cliente quedó "alucinado" — y por eso tienen muy buen concepto del equipo: el humano cubre la función de arquitectura aunque no sea su rol nominal.
