# W2M — grafos cíclicos en BBDD: bucles infinitos por IDs inconsistentes

En las BBDD de W2M, los **hoteles tenían múltiples IDs en distintas plataformas** (datos no actualizados consistentemente entre sistemas). Esto producía **bucles infinitos** al recorrerse el grafo de relaciones hotel→sistema→hotel. Resuelto con **algoritmos específicos** de detección y rotura de ciclos. El departamento de arquitectura del cliente quedó "alucinado" al ver la solución — y esa es una de las razones por las que el cliente tiene buen concepto del equipo: el humano cubre función de arquitectura aunque no sea su rol nominal.

## Filosofías que sostiene

- [Realidad ingenieril — el aparato invisible](../filosofia/realidad-ingenieril-aparato-invisible.md)
- [Elevar en vez de parchear](../filosofia/elevar-en-vez-de-parchear.md)
