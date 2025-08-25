# Material presentado como parte del curso

1. Descripción general del curso (`2025.08.12`):
   [Presentación](./00_presentacion.pdf)
2. Primer acercamiento (`2025.08.14`): Seguimos una _vieja_ presentación
   mía (modificada por última vez en 2008): [Seguridad en redes: ¿qué es?
   ¿cómo lograrla?](./01_seg_en_redes.pdf) → **¿Qué es la seguridad de la
   información?** y **Características de un sistema seguro**
3. Componentes básicos de la seguridad informática: Vamos siguiendo el
   discurso del capítulo 1 del libro [Introduction to Computer
   Security](https://www.oreilly.com/library/view/introduction-to-computer/0321247442/),
   de Matt Bishop. → **Propiedades de la seguridad de la información**

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

4. Seguiremos algunos textos para hablar de la **Seguridad informática capa
   a capa**. Algunas ideas:
   - [7 Layers of Cybersecurity Explained: A Complete
     Guide](https://axiomq.com/blog/7-layers-of-cybersecurity-explained-a-complete-guide/)
   - [Defense in Depth – The Layered Approach to
     Cybersecurity](https://cisotimes.com/defense-in-depth-the-layered-approach-to-cybersecurity/)
   - [What is layered security? A complete
     guide](https://www.comparitech.com/antivirus/what-is-layered-security/)
   Algunos artículos para trabajar más *en serio*:
   - Tillwick, Olivier (2004): [A layered security architecture: Design
     issues](http://martinolivier.com/open/lasa.pdf) Buena introducción
     general, definiciones basadas en los “servicios de seguridad”, “flujos
     de trabajo”, presenta propuesta genérica de capas.
   - Yildiz, Abawajy, Ercan y Bernoth (2009): [A Layered Security Approach
     for Cloud Computing
     Infrastructure](https://ieeexplore.ieee.org/iel5/5379703/5381549/05381731.pdf?casa_token=6mUhYsjCP6UAAAAA:LCTHnDK33_PBREtHTIHyKhw8cA4ALXig0j4RFlSTJWjy-DOQ0kmIn_LfS_Mb1MzzSiy1fI_V-w)
     presenta capas bastante diferentes, especializándose en el enfoque de
     “cloud computing”
   - Shiu, Chang, Wu, Huang, Chen (2011): [Physical Layer Security in
     Wireless Networks: A
     Tutorial](https://ieeexplore.ieee.org/iel5/7742/5751283/05751298.pdf)
     Separan diferentes tipos de ataque sobre sus diferentes
     características, detallan los servicios de seguridad que pueden
     aplicarse a cada uno.

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
