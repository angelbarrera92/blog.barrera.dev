---
title: IDP en la empresa
date: 2022-12-15
tags:
    - empresa
    - cultura
    - tecnología
cover: images/idp-in-the-enterprise.jpg
---

Hace unas semanas, dediqué algún tiempo a entender cómo se podía implantar un IDP en la empresa. Encontré algunos artículos y vídeos útiles, pero aún me quedaban algunas preguntas sin resolver. En particular, quería saber **cómo debe implantarse un IDP en un entorno político y lleno de silos**. También quería saber cómo hacer frente a la inevitable resistencia al cambio de los distintos departamentos.

> IDP significa **Plataforma de Desarrollo Interno**.

<!--more-->

[Aquí encontrarás el enfoque optimista de cómo implantar un IDP](https://github.com/angelbarrera92/idp-enterprise-research/blob/main/outcome.md), por desgracia, supone que la organización está bien estructurada y que **las personas están dispuestas a cambiar**, incluidos los mandos intermedios, los directores y los equipos de desarrollo.

Desgraciadamente, este no es el caso en la mayoría de las organizaciones. La realidad es que **la mayoría de las organizaciones están compartimentadas y son políticas**, y la gente no está dispuesta a cambiar, peor aún en tiempos de crisis económica. Por eso decidí escribir este artículo, para compartir mi punto de vista después de hablar con algunas personas del sector en la misma situación.

#### La situación

Es casi *2023*, y todas las industrias están digitalizadas, desde la venta al por menor a los bancos, comercios, y gobiernos por lo que es un hecho que **necesitamos ingenieros para dirigir una sociedad moderna.**

La mayoría de estas empresas *tienen éxito* en la adopción de la nube. Algunas de ellas están [volviendo a on-prem](https://www.channelpronetwork.com/article/return-prem), pero ese es un tema que me gustaría tratar en otro post.

Las empresas pasaron de *on-premises* al *cloud*. Algunas de ellas intentaron seguir los mismos procedimientos y procesos que seguían antes en sus centros de datos. Eso no funcionó, los ingenieros tenían dificultades para desarrollar e implementar los proyectos para los que estaban contratados, lo que provocó que los directivos y mandos intermedios no vieran ninguna mejora al pasar a la nube.

Llegados a este punto, tenían dos opciones:

- Seguir operando como lo estaban haciendo asumiendo que la nube no les iba a proporcionar mayores beneficios.
- Cambiar la forma de trabajar adoptando la flexibilidad de la nube.

Aquellas empresas que adoptaron el segundo punto, tuvieron que sustituir ciertos roles y procesos en la empresa.
Esto podría conllevar cambios significativos en la estructura de gestión de la empresa:

- ¿Quién gestiona el acceso a la nube?
- ¿Quién se ocupa de las cuentas en la nube?
- ¿Pueden los empleados utilizar cualquier servicio en la nube?
- ¿Quién se encarga de gestionar el cortafuegos de las instancias en la nube?
- ¿Y la facturación?

Como puedes imaginar, esto ha causado muchas dificultades a las empresas. Estos cambios *sólo* afectan a algunos departamentos de TI que adoptan procesos de automatización y prestan servicios a los desarrolladores.

##### Desarrolladores

Los desarrolladores, *en su día*, se centraban en desarrollar los requisitos del negocio. Luego, empujan el código a otro lugar, **trabajo hecho**.

Todos estamos de acuerdo en que **eso no es suficiente**. Desafortunadamente, **no hay consenso sobre lo que es suficiente** para un desarrollador.

- ¿Debe un desarrollador ocuparse de un pipeline?
- ¿Es consciente el desarrollador de los pasos que debe seguir el pipeline?
- ¿Debe el desarrollador ser consciente de la seguridad del *pipeline/código/infraestructura/datos*?

**Los desarrolladores quieren centrarse en escribir código y ofrecer valor de negocio**, en lugar de preocuparse por la infraestructura y el despliegue.

Es casi 2023, *en la nube*, con *contenedores*, con *APIs*, con *vulnerabilidades*, *contratistas*, *equipos de desarrollo internos*, y la *CNCF*.

##### CNCF

Nos trajo muchas herramientas y mucha confusión. Quiero decir, *Kubernetes*, *Prometheus*, *linkerd*, y otros proyectos son **maravillosos**. Desafortunadamente, cada proyecto alojado en el CNCF es una pieza de software que no hace nada por sí sola. Así que, **necesitas entender cómo usarlos, y necesitas saber cómo integrarlos.**

Esto no es fácil, **¿Es algo de lo que debe ocuparse el desarrollador?**.

La CNCF es la principal razón por la que las empresas invierten hoy en equipos de plataforma.

#### Consecuencias

La incorporación a la empresa/proyecto es un coñazo, tanto para el empleado como para el empresario:

- El empleado tiene que entender un montón de tecnologías diferentes y cómo se han implementado en la empresa/proyecto.
- Para el empleador, intentar encontrar un buen ingeniero en el mercado actual es una quimera. Tendrías que pagarles mucho ya que exiges del ingeniero muchos conocimientos. Sin olvidar que estamos en plena crisis económica.

No olvides el offboarding. **Los ingenieros quieren ser ingenieros, ¿verdad?** Así que si encuentran mejores oportunidades dentro de la misma empresa o fuera de ella, un ingeniero perseguirá esas oportunidades, por lo que acabarás con proyectos/productos inacabados.

Entonces, quita los permisos para ese ingeniero en particular, e **intenta incorporar a un nuevo empleado** en el proyecto/producto estos días...

##### microplataformas

Encontrarás **microplataformas** en diferentes equipos. *¿Qué es esto?*

Son frameworks que los desarrolladores avanzados del equipo desarrollan para **estandarizar la forma de trabajar** de su equipo, ya se están dando cuenta de que hay un problema de estandarización en la empresa en la que están trabajando.

*¿Cuál es el problema inevitable?*

No tienen suficiente contexto para implementar correctamente la *(micro)* plataforma, y probablemente podrían estar ligados a ciertos servicios que la empresa podría estar dando *(sistema de tickets, alertas, ejecución, métricas...)* y causará mucha fricción con los equipos de TI *(infra, plataforma, nube, seguridad....)*.

Me parece claro; los equipos están desarrollando su forma de desarrollar. **Entonces significa que hay un requerimiento potencial en la empresa**, y esto es estandarizar la forma de desarrollar *(IDP)*.

#### La fea verdad

La razón principal por la que no existe una única plataforma de desarrollo interno no tiene que ver con la tecnología, hay un número ingente de tecnologías listas para integrarse y cubrir la mayoría de los casos de uso que puedes ver en tu empresa.

*Entonces, ¿cuál es el problema?* **The middle management.**

En una empresa tradicional, verá una estructura organizativa bien definida con múltiples niveles de gestión. Desde el nivel C hasta abajo puedes encontrar 3-4-5 niveles de gestión *(incluso más; cuanto más grande sea la empresa, más niveles encontrarás)*.

Cada directivo se preocupa por X empleados y/o directivos.
**Cuantos más informes recibe el directivo, más "importante" es para la empresa**, al menos, esto es lo que podemos ver en este tipo de grandes empresas. Además, están acostumbrados a trabajar por proyectos, prestando servicios a distintas áreas. Así que es de esperar que interactúen dentro de las áreas a través de tickets/formularios...

Entonces... ¿Qué pasaría si alguien intenta implementar un IDP que involucra a muchos departamentos diferentes?

{{< image src="/images/IDPCapabilities.png" alt="Capacidades IDP" position="center" style="border-radius: 8px;" >}}

Los mandos intermedios podrían tomarse esto *(y lo hacen)* como un ataque a sus responsabilidades.

#### Conclusión

No tengo una bala de plata, pero tengo algunas ideas que podrían ayudarte a empezar a pensar en este tema.

- **Eche un vistazo a su entorno**; ¿Su jefe es consciente de la situación actual? Si no es así, intenta explicar la situación a tu jefe.
- **Empieza por los desarrolladores**. Los desarrolladores son los que van a utilizar la plataforma, por lo que deben ser ellos los que definan los requisitos y las capacidades de la plataforma. **Trátelos como a sus clientes.
- **Empezar poco a poco**. Empieza con un equipo pequeño e intenta implantar una microplataforma que puedan utilizar unos pocos equipos. Después, intenta ampliar la plataforma a otros equipos presentando las ventajas de utilizar esta plataforma a tu jefe.
- **Empieza por lo básico**. Empieza por lo básico e intenta implantar una plataforma que puedan utilizar todos los equipos de la empresa.

Deberías presentar junto con tu jefe las ventajas de utilizar la plataforma a los demás jefes.
Deberías ser capaz de mostrarles cómo la plataforma puede ayudarles a mejorar sus procesos y cómo puede ayudarles a mejorar su forma de trabajar.

**Implementada con éxito, ahorrará mucho dinero a la empresa**.
