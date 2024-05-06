## Monedero

### Contexto

Este repositorio contiene el código de un _monedero virtual_, al que podemos agregarle y quitarle dinero, a través 
de los métodos `Monedero.sacar` y `Monedero.poner`, respectivamente. 
Pero hay algunos problemas: por un lado el código no está muy bien testeado, y por el otro, hay numeros _code smells_. 

### Consigna

Tenés seis tareas: 

 1. :fork_and_knife: Hacé un repositorio usando este template (presionando desde Github el botón _use this template_)
 2. :arrow_down: Descargalo y construí el proyecto, utilizando `maven`
 2. :nose: Identificá y anotá todos los _code smells_ que encuentres 
 3. :test_tube: Agregá los tests faltantes y mejorá los existentes. 
     * :eyes: Ojo: ¡un test sin ningún tipo de aserción está incompleto!
 4. :rescue_worker_helmet: Corregí smells, de a un commit por vez. 
 5. :arrow_up: Subí todos los cambios a tu _fork_
 6. :bug: Activá los issues de Github desde https://github.com/TU_GITHUB_USERNAME/dds-monedero-java8/settings así podemos darte nuestras devoluciones

### Tecnologías usadas

* Java 17.
* JUnit 5. :warning: La versión 5 de JUnit es la más nueva del framework y presenta algunas diferencias respecto a la versión "clásica" (JUnit 4). Para mayores detalles, ver:
    *  [Apunte de herramientas](https://docs.google.com/document/d/1VYBey56M0UU6C0689hAClAvF9ILE6E7nKIuOqrRJnWQ/edit#heading=h.dnwhvummp994)
    *  [Entrada de Blog (en inglés)](https://www.baeldung.com/junit-5-migration)
    *  [Entrada de Blog (en español)](https://www.paradigmadigital.com/dev/nos-espera-junit-5/)
* Maven 3.3 o superior

### Code Smels encontrados

Medium: Read of unwritten field prenda in ar.edu.utn.frba.dds.Item.importe() [ar.edu.utn.frba.dds.Item] At Item.java:[line 8] NP_UNWRITTEN_FIELD
Unwritten field: ar.edu.utn.frba.dds.Item.prenda [ar.edu.utn.frba.dds.Item] At Item.java:[line 8] UWF_UNWRITTEN_FIELD
Read of unwritten field ventas in ar.edu.utn.frba.dds.Negocio.ganaciasDe(Date) [ar.edu.utn.frba.dds.Negocio] At Negocio.java:[line 10] NP_UNWRITTEN_FIELD
Unwritten field: ar.edu.utn.frba.dds.Negocio.ventas [ar.edu.utn.frba.dds.Negocio] At Negocio.java:[line 10] UWF_UNWRITTEN_FIELD
Read of unwritten field items in ar.edu.utn.frba.dds.Venta.importe() [ar.edu.utn.frba.dds.Venta] At Venta.java:[line 11] NP_UNWRITTEN_FIELD
Unwritten field: ar.edu.utn.frba.dds.Venta.fecha [ar.edu.utn.frba.dds.Venta] At Venta.java:[line 15] UWF_UNWRITTEN_FIELD
Unwritten field: ar.edu.utn.frba.dds.Venta.items [ar.edu.utn.frba.dds.Venta] At Venta.java:[line 11] UWF_UNWRITTEN_FIELD
