# Cambio de nombre — del "agente" al "avatar"

Hito conceptual: el equipo deja de llamar "agente" a la pieza IA y empieza a llamarla **avatar**. Dos analogías guían el cambio: la película **Avatar** (Sully dentro del cuerpo na'vi — el cuerpo opera, pero el humano dirige desde dentro) e **Iron Man** (Tony Stark dentro del traje). El avatar **no es** el agente IA solo: es el sistema **humano + IA + estructura externa**. Cambiar el nombre cambia lo que se delega, lo que se verifica y dónde vive la responsabilidad.

## Filosofías que sostiene

- [Del agente al avatar](../filosofia/del-agente-al-avatar.md)
- [Avatar autoconsciente](../filosofia/avatar-autoconsciente.md)
- [Multi-avatar / multi-rol](../filosofia/multi-avatar-multi-rol.md)
- [Estados públicos no internos](../filosofia/estados-publicos-no-internos.md)
- [Analogía cloud antes de Istio](../filosofia/analogia-cloud-pre-istio.md)

```avatar-lang
@id: cambio-nombre-agente-a-avatar
state BORRADOR "En elaboración"
state PUBLICADO terminal "Publicado en avatar-mind"
action publicar: BORRADOR -> PUBLICADO {
  title: "publicar"
  description: "Documento registrado en avatar-mind"
  requires: BORRADOR
  produces: PUBLICADO
}
```
