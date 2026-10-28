# Historias de usuario de búsqueda

| Campo | Valor |
| --- | --- |
| Proyecto | Proyecto Simbiosis |
| Fecha | [27/10/2026] |
| Versión | 0.1 |
| Estado | Borrador |

## Fuentes comunes

- [Acta de UC-21 Buscar recetas](../captura/acta-acuerdos-uc-21-buscar-recetas.md), v1.1, Vigente.
- [Catálogo de requisitos](catalogo-requisitos.md), UR-08 y FR pertinentes.
- [Modelo de casos de uso](../modelos/modelo-casos-de-uso.md), UC-21.

## Épica de búsqueda

Como usuario, quiero buscar recetas mediante texto, para encontrar opciones adaptadas a mi situación alimentaria

**Estado:** descompuesta en US-01, US-02 y US-03. Conserva la necesidad conjunta.

## Justificación de la división

Cada historia abarca un criterio de búsqueda independiente que aporta un valor al usuario al filtrar el catálogo. Esto permite implementar la búsqueda sin depender de demás filtros.

## US-01

**Título:** Búsqueda de recetas por texto

Como usuario registrado, quiero buscar recetas introduciendo algún dato específico sobre esta, para encontrar recetas que coincidan con mi búsqueda.

**Fuentes:** UR-08; UC-21; FR85; acta, [apartado pertinente].

### Criterios de aceptación

- **CA-01.** Dado que existen las recetas "Ensalada de Zanahorias" y "Tarta de la abuela", cuando el usuario busca "abuela", entonces el sistema muestra "Tarta de la abuela" en los resultados solamente.
- **CA-02.** Dado que el catálogo no contiene ninguna receta con el término introducido por el usuario, entonces el sistema informa que no se han encontrado resultados.
- **CA-03.** Dado que existen las recetas "Jugo de naranja" y "Tarta de naranja", cuando el usuario busca "naranja", entonces el sistema muestra ambas recetas en los resultados.

## US-02

**Título:** Búsqueda de recetas por ingredientes incluidos

Como usuario registrado, quiero buscar recetas seleccionando ingredientes, para encontrar recetas que pueda preparar con los ingredientes que tengo

**Fuentes:** UR-08; UC-21; [FR 86]; acta, [apartado pertinente].

### Criterios de aceptación

- **CA-01.** Dado que existen las recetas "Tortilla de patacas" (ingredientes: huevo, patacas), y "Huevo frito" (ingredientes: huevo), cuando el usuario seleccione "huevo" y "patata" como ingredientes, entonces el sistema solo muestra la "Tortilla de paracas" 
- **CA-02.** Dado [situación], cuando [acción], entonces [resultado observable].
- **CA-03.** Dado [situación], cuando [acción], entonces [resultado observable].

## US-03

Como usuario registrado quiero excluir ingredientes de una búsqueda, para evitar recetas que contengan ingredientes que no quiero utilizar.

Como [rol], quiero [capacidad], para [beneficio].

**Fuentes:** UR-08; UC-21; [FR ]; acta, [apartado pertinente].

### Criterios de aceptación

- **CA-01.** Dado [situación], cuando [acción], entonces [resultado observable].
- **CA-02.** Dado [situación], cuando [acción], entonces [resultado observable].
- **CA-03.** Dado [situación], cuando [acción], entonces [resultado observable].

## Revisión INVEST

La revisión abarca US-01, US-02 y US-03. «Aplicado» indica si se ha realizado la comprobación. «Cumple» indica si todas las historias cumplen el criterio. Si alguna no lo cumple, indicar «No» e identificar la historia y el motivo en la justificación. Si no se ha realizado la comprobación o faltan datos, indicar «Pendiente» en «Cumple».

| Criterio | Pregunta de revisión | Aplicado | Cumple | Justificación |
| --- | --- | --- | --- | --- |
| Independiente | ¿Puede implementarse cada historia y ofrecer un resultado útil sin implementar antes las otras historias del conjunto? Puede compartir infraestructura con ellas. | [Sí/No] | [Sí/No/Pendiente] | [Historias y motivo] |
| Negociable | ¿Cada historia explica qué necesita la persona y deja margen para discutir los detalles de la solución, respetando los acuerdos confirmados? | [Sí/No] | [Sí/No/Pendiente] | [Historias y motivo] |
| Valiosa | ¿La parte «para…» de cada historia explica el beneficio que obtiene la persona al usar esa capacidad? | [Sí/No] | [Sí/No/Pendiente] | [Historias y motivo] |
| Estimable | ¿Están claros el alcance y los datos necesarios para estimar el trabajo de cada historia? | [Sí/No] | [Sí/No/Pendiente] | [Historias y motivo] |
| Pequeña | ¿Se centra cada historia en una única capacidad de alcance manejable? | [Sí/No] | [Sí/No/Pendiente] | [Historias y motivo] |
| Comprobable | ¿Los criterios de aceptación de cada historia describen acciones y resultados observables que permiten distinguir un comportamiento correcto de uno incorrecto? | [Sí/No] | [Sí/No/Pendiente] | [Historias y motivo] |

## Dudas pendientes

[Cuestiones pendientes de aclaración. Si no quedan cuestiones, indicar «Ninguna».]
