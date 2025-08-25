# Material presentado como parte del curso

1. Descripción general del curso (`2025.08.12`):
   [Presentación](./00_presentacion.pdf)
2. Primer acercamiento (`2025.08.14`): Seguimos una _vieja_ presentación
   mía (modificada por última vez en 2008): [Seguridad en redes: ¿qué es?
   ¿cómo lograrla?](./01_seg_en_redes.pdf)
3. Componentes básicos de la seguridad informática: Vamos siguiendo el
   discurso del capítulo 1 del libro [Introduction to Computer
   Security](https://www.oreilly.com/library/view/introduction-to-computer/0321247442/),
   de Matt Bishop.

   `2025.08.19`:
   - _La triada de la seguridad_, o los tres principales _aspectos_ o
     _servicios_ de la seguridad: Confidencialidad, Integridad,
     Disponibilidad

   - _Amenazas_, _Ataques_ (¿e _incidentes_?) Categorías de estos, y
     relación con la _triada_:
	 - _Divulgación_ (disclosure), _engaño_ (deception), _disrupción_
       (disruption), _usurpación_ (usurpation) ⇒ Shirey 1994: Security
       Architecture for Internet Protocols: A Guide for Protocol Designs
       and Standards (draft expirado de IRTF)

   `2025.08.21`:
   - _Amenazas_, _Ataques_ (¿e _incidentes_?), continuado
     - _Fisgoneo_ (snooping / eavesdropping / wiretapping)
     - _Modificación_ o _alteración_
     - Suplantación de identidad / enmascaramiento ⇒ MitM (_Man in the
       Middle_) ( ∈ _usurpación_;  ≠ _delegación_)
     - Repidio de origen / Negación de recepción
     - Demora / negación de servicio
   - Objetivos de la seguridad
     - Prevención
     - Detección
     - Recuperación ⇒ Vuelta al _estado confiado_; operación correcta _aún
       bajo ataque_
   - Políticas y mecanismos ⇒ Qué y cómo. Especificación, diseño e implementación..

# Temas adicionales abordados

...Tal vez porque el interés y la plática *caminaron naturalmente* hacia
allá, por pregunta expresa, por lo que sea — son temas que cubrimos en
clase, ¡y vale la pena mantener en mente!

Posiblemente esta sección no esté tan completa y bien ordenada, pero no la
olvidemos. ¿Falta algo por agregar? ¡Agréguenlo ustedes mismos! (o
recuérdenme que lo haga)

`2025.08.19`:
- ¿Que es la divulgación de información por canales laterales?
`2025.08.21`:
- El *modelo transitivo de confianza* PKI-CA:
  - El ataque *Heartbleed* (2014) y la exfiltración de llaves privadas
  - El *Certificate Authority Browser Forum* (CABF)
  - Algunos aspectos del ecosistema de las CAs, referencias a algunas
    *actividades hostiles* que se han registrado
