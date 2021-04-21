.. _ERPyA: http://erpya.com

.. _documento/tipo-documento:

**Tipo de Documento**
=====================

En ADempiere los tipos de documentos definen el comportamiento de los documentos que generan transacciones administrativas y contables de una empresa, adicional a ello permite personalizar el proceder fiscal y contable de cada uno.

Son creados con base en los procesos que gestiona ADempiere, en otras palabras, son utilizados durante todo el ciclo de vida de una empresa, contemplando múltiples procesos que van desde el proceso de manufactura, iniciando desde compra, recursos humanos y pasando por ventas, finanzas y control de gastos, hasta llegar a los resultados generados como asientos contables.

El presente material es elaborado por `ERPyA`_, explicará de forma eficiente al usuario la utilidad que representa la configuración de los tipos de documentos para nuestra localización Venezuela.

**Orden de Calidad** |Orden de Calidad|
---------------------------------------

Es un documento donde se establecen los requisitos con los que deben cumplir los productos y servicios, es utilizado para organizar, dirigir y controlar la producción de una determinada empresa, asegurando así la calidad de los productos y servicios a los clientes.

El objetivo de la elaboración de este documento radica en asegurar la calidad de los productos y servicios en tres (3) fases llevadas a cabo en las empresas, en la planificación de la producción, en la producción y en la distribución de los productos, para entregar a los clientes productos y servicios que satisfagan sus necesidades.

**Tipo de Documento Orden de Calidad**
**************************************

En ADempiere una orden de calidad refleja los lineamientos que debe cumplir el departamento de producción en cuanto a los productos y servicios elaborados para el consumo de los socios de negocios tipo clientes.

**Orden de Calidad**
~~~~~~~~~~~~~~~~~~~~

**Definición**

    Una orden de calidad se elabora previo a la planificación de lo que la empresa requiere que se produzca, sin embargo, se debe tomar en cuenta al momento de elaborar una orden de producción o de manufactura ya que se requiere que los materiales a utilizar sean de calidad para que la producción cumpla con lo establecido en el documento orden de calidad.

.. warning::

    Los productos realizados deben cumplir con los requerimientos de los clientes y satisfacer sus necesidades.

**Comportamiento**

    En ADempiere la orden de calidad se define según su comportamiento, a continuación se explica el proceder de una **Orden de Calidad**:

    +------------------------+-----------------+--------------------------------------------------+
    |         **Campo**      |    **Valor**    | **Comportamiento en ADempiere**                  |
    +========================+=================+==================================================+
    | Tipo de Documento Base:|Orden de Calidad | Genera una **Orden de Calidad** a una empresa.   |
    +------------------------+-----------------+--------------------------------------------------+
    | Documento Controlado:  |Si               | Mantiene una **Secuencia de Control**.           |
    +------------------------+-----------------+--------------------------------------------------+
    |Secuencia del Documento:|Orden de Calidad |Genera el número de secuencia establecido para el |
    |                        |                 |orden de los tipos de documentos de ADempiere,    |
    |                        |                 |configurado en la secuencia de documentos y es    |
    |                        |                 |incrementable en 1, en este caso la secuencia     |
    |                        |                 |comienza en 87.000 y su prefijo esta compuesto por|
    |                        |                 |las iniciales de su nombre "**ORC-**".            |
    +------------------------+-----------------+--------------------------------------------------+
    | Copias del Documento:  |1                | Establece el número de copias a imprimir.        |
    +------------------------+-----------------+--------------------------------------------------+

**Implicación en ADempiere**

    - Genera al departamento de producción una planificación de procesos a aplicar.
    - Garantiza productos de calidad cuando se cumple el documento en todas sus especificaciones.

**Implicación Fiscal**

Basado en la Norma Internacional ISO 9000:2015, Sistemas de gestión de la calidad — Fundamentos y vocabulario, donde indica en el items seis (6) referente a la planificación, lo siguiente:

**6.1 Acciones para abordar riesgos y oportunidades**

    6.1.1 Al planificar el sistema de gestión de la calidad, la organización debe considerar las cuestiones referidas en el apartado 4.1 y los requisitos referidos en el apartado 4.2, y determinar los riesgos y oportunidades que es necesario abordar con el fin de:

        - asegurar que el sistema de gestión de la calidad pueda lograr sus resultados previstos;
        - aumentar los efectos deseables;
        - prevenir o reducir efectos no deseados;
        - lograr la mejora.

    6.1.2 La organización debe planificar:

        - las acciones para abordar estos riesgos y oportunidades;
        - la manera de:
        - integrar e implementar las acciones en sus procesos del sistema de gestión de la calidad (véase 4.4.);
        - evaluar la eficacia de estas acciones.

        Las acciones tomadas para abordar los riesgos y oportunidades deben ser proporcionales al impacto potencial en la conformidad de los productos y los servicios.

        NOTA 1 Las opciones para abordar los riesgos pueden incluir: evitar riesgos, asumir riesgos para perseguir una oportunidad, eliminar la fuente de riesgo, cambiar la probabilidad o las consecuencias, compartir el riesgo o mantener riesgos mediante decisiones informadas.

        NOTA 2 Las oportunidades pueden conducir a la adopción de nuevas prácticas, lanzamiento de nuevos productos, apertura de nuevos mercados, acercamiento a nuevos clientes, establecimiento de asociaciones, utilización de nuevas tecnologías y otras posibilidades deseables y viables para abordar las necesidades de la organización o las de sus clientes.

**6.2 Objetivos de la calidad y planificación para lograrlos**

    6.2.1 La organización debe establecer objetivos de la calidad para las funciones y niveles pertinentes y los procesos necesarios para el sistema de gestión de la calidad.

    Los objetivos de la calidad deben:

        - ser coherentes con la política de la calidad;
        - ser medibles;
        - tener en cuenta los requisitos aplicables;
        - ser pertinentes para la conformidad de los productos y servicios y para el aumento de la satisfacción del cliente;
        - ser objeto de seguimiento;
        - comunicarse;
        - actualizarse, según corresponda.

    La organización debe mantener información documentada sobre los objetivos de la calidad.

    6.2.2 Al planificar cómo lograr sus objetivos de la calidad, la organización debe determinar:

        - qué se va a hacer;
        - qué recursos se requerirán;
        - quién será responsable;
        - cuándo se finalizará;
        - cómo se evaluarán los resultados.

**6.3 Planificación de los cambios**

    Cuando la organización determine la necesidad de cambios en el sistema de gestión de la calidad, estos cambios se deben llevar a cabo de manera planificada (véase 4.4).

    La organización debe considerar:

        - el propósito de los cambios y sus consecuencias potenciales;
        - la integridad del sistema de gestión de la calidad;
        - la disponibilidad de recursos;
        - la asignación o reasignación de responsabilidades y autoridades.
