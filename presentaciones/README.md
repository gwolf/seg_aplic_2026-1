* Material presentado como parte del curso

1. Descripción general del curso (2025.08.12):
   [Presentación](./00_presentacion.pdf)
2. Primer acercamiento (2025.08.14): Seguimos una _vieja_ presentación mía
   (modificada por última vez en 2008): [Seguridad en redes: ¿qué es? ¿cómo
   lograrla?](./01_seg_en_redes.pdf)
3. Componentes básicos de la seguridad informática: Vamos siguiendo el
   discurso del capítulo 1 del libro [Introduction to Computer
   Security](https://www.oreilly.com/library/view/introduction-to-computer/0321247442/),
   de Matt Bishop.

   2025.08.19:
   - _La triada de la seguridad_, o los tres principales _aspectos_ o
     _servicios_ de la seguridad: Confidencialidad, Integridad,
     Disponibilidad

   - _Amenazas_, _Ataques_ (¿e _incidentes_?) Categorías de estos, y
     relación con la _triada_:
	 - _Divulgación_ (disclosure), _engaño_ (deception), _disrupción_
       (disruption), _usurpación_ (usurpation) ⇒ Shirey 1994: Security
       Architecture for Internet Protocols: A Guide for Protocol Designs
       and Standards (draft expirado de IRTF)
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
