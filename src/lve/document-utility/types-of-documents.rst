.. _ERPyA: http://erpya.com

.. |Orden de Calidad| image:: resources/certificado.png
.. |Insumo del Proyecto| image:: resources/insumo.jpeg
.. |Orden de Producción Planeada| image:: resources/nuevo1.png
.. |Orden de Manufactura| image:: resources/nuevo1.png
.. |Producción| image:: resources/produccion.jpg
.. |Inventario| image:: resources/inventario.png
.. |Orden de Distribución| image:: resources/certificado.png
.. |Movimiento de Material| image:: resources/movimientointerno.png
.. |Orden de Venta| image:: resources/orden.png
.. |Cuentas por Cobrar| image:: resources/cuentas.png
.. |Nota de Crédito de Cuentas por Cobrar| image:: resources/nota.png
.. |Cobros| image:: resources/cobro.jpg
.. |Ventas| image:: resources/venta.png
.. |Requisición| image:: resources/requisiciones.jpeg
.. |Orden de Compra| image:: resources/orden.png
.. |Cuentas por Pagar| image:: resources/cuentas.png
.. |Nota de Crédito de Cuentas por Pagar| image:: resources/nota.png
.. |Comisión de Ventas| image:: resources/comision.png
.. |Selección de Pago de Cuentas por Pagar| image:: resources/seleccion.jpg
.. |Pagos| image:: resources/pago.png
.. |Asignación de Pagos| image:: resources/asignacion.png
.. |Compras| image:: resources/compra.jpg
.. |Asignar OC| image:: resources/seleccion.jpg
.. |Extracto Bancario| image:: resources/extracto.jpeg
.. |Nómina| image:: resources/nomina.png
.. |Selección de Pago Nómina| image:: resources/seleccion.jpg
.. |Orden de Mantenimiento| image:: resources/mantenimiento.jpeg
.. |Depreciación de Activos| image:: resources/depreciacion.jpeg
.. |Adición de Activos| image:: resources/adicion.jpeg
.. |Venta de Activos| image:: resources/activos.jpeg
.. |Nota de Contabilidad| image:: resources/nota.png
.. |Calendario1| image:: resources/calendario.png
.. |Calendario2| image:: resources/calendario2.png
.. |Calendario3| image:: resources/calendario3.png


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

**Insumo del Proyecto** |Insumo del Proyecto| 
---------------------------------------------

Es el documento donde se detallan todos los materiales que el departamento de producción vaya a utilizar para elaborar un determinado proyecto, es decir, los materiales fundamentales para logar una producción.

Los insumos varían dependiendo del producto que la empresa vaya a producir y la cantidad total planificada del mismo.

**Tipo de Documento Insumo de Proyecto**
****************************************

En ADempiere el documento permite ayudar al departamento de producción de la empresa en cuanto al control y la organización necesaria para la producción, el mismo es definido según su comportamiento y especificado a continuación.

**Insumo de Proyecto**
~~~~~~~~~~~~~~~~~~~~~~

**Definición**

    Es un documento necesario para la elaboración de la orden de producción o de manufactura, considerándose la base para la planificación de las mismas, dando inicio al proceso de producción que se realiza en una determinada empresa.

.. warning:: 

    El documento de insumos del proyecto contiene de manera detallada la cantidad de insumos de calidad con los que cuenta la empresa para iniciar el proceso de producción. 

**Comportamiento**

    En ADempiere el insumo de proyecto se define según su comportamiento, a continuación se explica el proceder del **Insumo de Proyecto**:

    +------------------------+------------------+--------------------------------------------------+
    |         **Campo**      |     **Valor**    | **Comportamiento en ADempiere**                  |
    +========================+==================+==================================================+
    | Tipo de Documento Base:|Insumo de Proyecto|Genera un documento de **Insumo de Proyecto** a   |
    |                        |                  |una empresa.                                      |
    +------------------------+------------------+--------------------------------------------------+
    | Copias del Documento:  |1                 | Establece el número de copias a imprimir.        |
    +------------------------+------------------+--------------------------------------------------+

**Implicación en ADempiere**

    - Genera la información necesaria sobre los insumos disponibles para un proyecto.
    - Permite la elaboración de una orden de producción planeada.
    - Permite la elaboración de una orden de manufactura.

**Implicación Fiscal**

    No posee implicación fiscal por no ser un documento legal.

**Orden de Producción Planeada** |Orden de Producción Planeada| 
---------------------------------------------------------------

Una orden de producción parte del proceso de planificación de producción de una determinada empresa, es elaborada basandose en los materiales o insumos de producción con los que cuenta la misma. Una vez ya planificada la producción se procede a realizar la autorización, o bien, la orden de producción.

Por medio de este documento se lleva un control de los materiales, gastos, y el tiempo empleado por los trabajadores o maquinarias. Adicional a ello, indica los productos y la cantidad que se debe producir en un tiempo estimado.

**Tipo de Documento Orden de Producción Planeada**
**************************************************

En ADempiere este tipo de documento permite generar al departamento de producción la información necesaria para que sea distribuido correctamente el trabajo y puedan comenzar con el proceso de producción.

**Orden de Producción Planeada**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Definición**

    Es un tipo de documento que representa la autorización que realiza el jefe de producción de una empresa, el mismo se basa en los materiales adquiridos para indicar a los trabajadores el estimado de productos manufacturados que se debe cumplir en el día o en el mes.

.. warning:: 

    Es un documento utilizado por las empresas al comenzar su producción, autorizando por medio de este el inicio de la misma.


**Comportamiento**

    En ADempiere la orden de producción planeada se define según su comportamiento, a continuación se explica el proceder de una **Orden de Producción Planeada**:

    +------------------------+------------------+--------------------------------------------------+
    |         **Campo**      |    **Valor**     | **Comportamiento en ADempiere**                  |
    +========================+==================+==================================================+
    |Tipo de Documento Base: |Manufacturing     |Genera un documento de **Orden de Producción**    |
    |                        |Planned           |**Planeada** a la empresa.                        |
    +------------------------+------------------+--------------------------------------------------+
    |Documento Controlado:   |Si                |Mantiene una **Secuencia de Control**.            |
    +------------------------+------------------+--------------------------------------------------+
    |Copias del Documento:   |1                 |Establece el número de copias a imprimir.         |
    +------------------------+------------------+--------------------------------------------------+

**Implicación en ADempiere**

    - Autoriza una producción determinada.
    - Controla la cantidad de materiales, gastos y tiempo invertido para la producción.
    - Garantiza una buena distribución de la producción.

**Implicación Fiscal**

    No posee implicación fiscal por no ser un documento legal.


**Orden de Manufactura** |Orden de Manufactura| 
-----------------------------------------------

Es un documento en el que se especifican los productos o servicios a realizar, así como la cantidad de los mismos. En una orden de manufactura se establecen los materiales necesarios y las fechas de comienzo y fin de la producción, de igual manera la fecha de entrega del mismo.

**Tipo de Documento Orden de Manufactura**
******************************************

En ADempiere una orden de manufactura autoriza la producción en planta y específica cada detalle necesario para la misma. Es definido según su comportamiento y explicado a continuación.

**Orden de Manufactura**
~~~~~~~~~~~~~~~~~~~~~~~~

**Definición**

    Es un documento utilizado por la empresa para controlar y dar seguimiento a todo el proceso de manufactura que realiza la misma a la hora de elaborar sus productos y servicios.

.. warning:: 

    Es un documento utilizado por las empresas al comenzar su producción, autorizando por medio de este el inicio de la misma.

**Comportamiento**

    En ADempiere la orden de manufactura se define según su comportamiento, a continuación se explica el proceder de una **Orden de Manufactura**:

    +------------------------+------------------+--------------------------------------------------+
    |         **Campo**      |    **Valor**     | **Comportamiento en ADempiere**                  |
    +========================+==================+==================================================+
    |Tipo de Documento Base: |Orden de          |Genera un documento de **Orden de Manufactura** a |
    |                        |Manufactura       |la empresa.                                       |
    +------------------------+------------------+--------------------------------------------------+
    | Documento Controlado:  |Si                |Mantiene una **Secuencia de Control**.            |
    +------------------------+------------------+--------------------------------------------------+
    |Secuencia del Documento:|Orden de          |Genera el número de secuencia establecido para el |
    |                        |Manufactura       |orden de los tipo de documentos de ADempiere,     |
    |                        |                  |configurado en la secuencia de documentos y es    |
    |                        |                  |incrementable en 1, en este caso la secuencia     |
    |                        |                  |comienza en 80.000 y su prefijo esta compuesto por|
    |                        |                  |las iniciales de su nombre "**OM-**".             |
    +------------------------+------------------+--------------------------------------------------+
    | Copias del Documento:  |1                 |Establece el número de copias a imprimir.         |
    +------------------------+------------------+--------------------------------------------------+

**Implicación en ADempiere**

    - Autoriza una producción determinada.
    - Controla la cantidad de materiales, gastos y tiempo invertido para la producción.
    - Garantiza una buena distribución de la producción.

**Implicación Fiscal**

    No posee implicación fiscal por no ser un documento legal.

**Producción de Material** |Producción|
---------------------------------------

Es el resultado de varias fases de trabajo que se llevan a cabo en una determinada empresa, también es llamado proceso de manufactura, esta es la base o el recurso principal para el ingreso monetario.

Todos los procesos que se llevan a cabo en una empresa estan relacionados directa o indirectamente con el mismo, en tal sentido, la mano de obra puede ser considerada como directa o indirecta dentro del proceso.

La manufactura es originada desde una planificación previa, estimando metas u objetivos de producción que serán producto de control dentro de los turnos que conforman la producción, el resultado de los mismos determinan la estabilidad de una empresa y la disponibilidad de los productos terminados para la venta.

**Tipo de Documento Producción de Material**
********************************************

En ADempiere una producción de material define los productos o servicios elaborados por una determinada empresa, y su proceder es único en cada documento generado por el mismo.

**Producción de Material**
~~~~~~~~~~~~~~~~~~~~~~~~~~

**Definición**

    Es el documento que refleja el resultado obtenido de la producción realizada por la empresa, los productos o servicios producidos son la base para el ingreso monetario, los mismos deben pasar por control de calidad antes de ser expuestos al cliente, cuando la producción se trata de alimentos para el consumo humano, el cuidado y tratado del producto debe ser mayor.

    En Venezuela, el ente encargado de regir el proceso de producción en el caso de los alimentos es el ministerio del poder popular para la alimentación.

.. warning:: 

    La producción de material no puede ser expuesta hasta que el departamento de control de calidad indique que es un producto o servicio competente para salir de la empresa en la cual fue producido.

**Comportamiento**

    En ADempiere la producción de material se define según su comportamiento, a continuación se explica el proceder de **Producción de Material**:

    +------------------------+------------------+--------------------------------------------------+
    |         **Campo**      |    **Valor**     | **Comportamiento en ADempiere**                  |
    +========================+==================+==================================================+
    |Tipo de Documento Base: |Producción de     |Genera un documento de **Producción de Material** |
    |                        |Material          |a la empresa.                                     |
    +------------------------+------------------+--------------------------------------------------+
    |Copiar Número de        |                  |**Copia el número de documento en el reverso** en |
    |Documento en Reverso:   |Si                |lugar de generar un nuevo número agregándole el   |
    |                        |                  |símbolo **^** al final del número de documento,   |
    |                        |                  |además el monto del documento pasa a **negativo**.|
    +------------------------+------------------+--------------------------------------------------+
    |Copias del Documento:   |1                 |Establece el número de copias a imprimir.         |
    +------------------------+------------------+--------------------------------------------------+

**Implicación en ADempiere**

    - Refleja en ADempiere la cantidad producida como producto en existencia.
    - Permite un ingreso monetario a cambio de este por medio de ventas.
    - Se encuentra disponible automaticamente para las ventas de la empresa.

**Implicación Fiscal**

Basado en el decreto N° 5.246 publicado en la gaceta oficial N° 38.654 con fecha del 28 de marzo del 2007 donde estipula en su artículo 26 lo siguiente:

    **Artículo 26:** Son competencias del ministerio del poder popular para la alimentación:

    - La regulación, formulación, seguimiento y evaluación de políticas, planificación y realización de las actividades del Ejecutivo Nacional en materia de comercio, industria, mercadeo y distribución de alimentos. 

    - La regulación, formulación, seguimiento y evaluación de políticas, planificación y realización de las actividades del Ejecutivo Nacional en materia de seguridad alimentaria, en coordinación con los Ministerios del Poder Popular para la Agricultura y Tierras y del Poder Popular para el Comercio. 

    - La regulación, formulación, seguimiento y evaluación de políticas, la planificación y realización de las actividades del Ejecutivo Nacional, en materia de seguridad alimentaria, en coordinación con los Ministerios del Poder Popular para la Agricultura y Tierras y del Poder Popular para las Industrias Ligeras y Comercio; 

    - La regulación, formulación, seguimiento y evaluación de políticas, planificación y realización de las actividades del Ejecutivo Nacional en materia de recepción, almacenamiento, depósito, conservación, transporte, distribución, entrega, colocación y consumo de alimentos. 

    - La planificación, coordinación, seguimiento y evaluación de las actividades empresariales del Estado en el sector de los alimentos, de la alimentación. 

    - La participación en las negociaciones internacionales en materia de alimentos, en coordinación con los Ministerios del Poder Popular para la Agricultura y Tierras, del Poder Popular para el Comercio, y del Poder Popular para Relaciones Exteriores. 

    - Dirigir la política de comercio exterior en materia de alimentos, alimentación, en coordinación con los Ministerios del Poder Popular para la Agricultura y Tierras, del Poder Popular para el Comercio, y del Poder Popular para Relaciones Exteriores. 

    - La planificación, formulación, seguimiento y evaluación de políticas, en materia de calidad de alimentos, de alimentación, en coordinación con el Ministerio del Poder Popular para la Salud. 

    - La regulación, formulación y promoción de estrategias, conjuntamente con los Ministerios del Poder Popular para la Agricultura y Tierras, y del Poder Popular para el Comercio, para equilibrar la oferta y la demanda de los circuitos agroalimentarios; así como la regulación de los productos alimenticios, completando los ciclos de producción y comercialización. 

    - La formulación, planificación, coordinación, seguimiento y realización de Planes Especiales de Alimentación, de carácter excepcional. 

    - La concertación, análisis y la fijación de precios y tarifas, de productos y servicios alimenticios y nutricionales, en coordinación con los órganos y entes competentes en la materia. 

    - Ejercer la rectoría en materia de inspección, vigilancia, fiscalización y sanción sobre actividades de almacenamiento agrícola y sus actividades conexas, a través del órgano competente. 

    - Lo relativo a la administración, operación, explotación silos, frigoríficos, almacenes y depósitos agrícolas, propiedad del Estado de conformidad con la Ley. 

    - La regulación expedición de permisos, autorizaciones, licencias, certificados y demás trámites y actos necesarios en materia de exportación e importación en el sector de alimentos, alimentación y nutrición. 

    - Lo relativo al almacenamiento, oferta, transporte y comercio de vegetales o animales o sus partes. 

    - Coordinar con los organismos competentes, la formulación, coordinación, seguimiento y evaluación de las políticas para la adquisición, instalación y administración de maquinarias y equipos necesarios para la producción y comercialización de alimentos. 

    - La dirección, administración y manejo de programas de compensaciones para el desarrollo competitivo para el sector alimentos. 

    - La planificación, coordinación, seguimiento y evaluación de políticas de financiamiento en el sector de producción y comercio de alimentos.

    - La inspección y vigilancia del ejercicio de toda profesión y actividad relacionada con los alimentos, la alimentación. 

    - Formular, planificar y hacer seguimiento a la política comunicacional en materia de calidad y consumo de alimentos, su publicidad y divulgación a la población venezolana, en coordinación con la planificación y políticas de comunicación e información dictadas por el Ministerio del Poder Popular para la Comunicación e Información, y sin perjuicio de las competencias que le corresponden a este Ministerio, de conformidad con el artículo 24 del presente Decreto. 

    - Las demás que le atribuyan las Leyes y otros actos normativos. 
