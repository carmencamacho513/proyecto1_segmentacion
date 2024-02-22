# 🍭 Herramientas, lenguajes e insumos

#### 1.1 Herramientas y/o plataformas <a href="#id-11herramientasyoplataformas" id="id-11herramientasyoplataformas"></a>

En este proyecto vas a utilizar tres herramientas de _Google_, una para el manejo de los datos, una para crear presentaciones y otra para la visualización del resultado de tu trabajo (en el hito 3):

* _Google Sheets_
* _Google Slides_
* _Looker Studio_

#### 1.2 Lenguajes <a href="#id-12lenguajes" id="id-12lenguajes"></a>

En este proyecto utilizarás solamente las fórmulas de _Google Sheets_.

#### 1.3 Insumos <a href="#id-13insumos" id="id-13insumos"></a>

El insumo con el que cuentas es un _dataset_ con tres tablas, cada una originalmente en formato CSV, pero ya cargada y convertida en un archivo de _Google Sheets_, a los cuales tendrás acceso a través de los siguientes enlaces:

* [Tabla de clientes](https://docs.google.com/spreadsheets/d/1eJxIxHTx9PzQO8f05ZcYhMkDB6yyJhtja8pktGF-Gzg/edit?usp=sharing)
* [Tabla de transacciones](https://docs.google.com/spreadsheets/d/1dD2UF-XPWjPu7pkApGCQ1uIIVA0gAcZ-Qk4LPmxX10A/edit?usp=sharing)
* [Tabla resumen\_compras](https://docs.google.com/spreadsheets/d/1Tkg0lYsAiwu6CB6slktwUMdayWTvBq80SyX16r-xEVA/edit?usp=sharing)

Antes de describir los datos en detalle, es importante que conozcas qué es un _dataset_ y cuáles son los tipos de archivos que puede contener.

Un _dataset_ (_data_: datos + _set_: conjunto) es un conjunto de datos habitualmente tabulados. En el caso de datos tabulados, más conocidos como tablas, los valores para cada una de las variables están organizados como columnas, como por ejemplo el año de nacimiento, nivel de educación y estado civil de una persona, que corresponden a cada miembro del conjunto de datos, que están organizados en filas, como podemos ver en la siguiente imagen:

![image](https://drive.google.com/uc?id=1v1DYao-OidrxxsaVTu7spGZsULXY\_Iui)

El conjunto de datos también puede consistir en una colección de documentos o de archivos en diferentes formatos como CSV (_Comma-Separated Values_), XLS (_Excel_) etc.

El _dataset_ (conjunto de datos) de este proyecto cuenta con una tabla de datos de clientes, una de las transacciones de esos clientes y una con el resumen de compras hechas por los clientes en el periodo de 2020-07-30 hasta 2022-06-29 (formato año-mes-día), conteniendo las siguientes variables respectivamente:

*   [Tabla de clientes](https://docs.google.com/spreadsheets/d/1eJxIxHTx9PzQO8f05ZcYhMkDB6yyJhtja8pktGF-Gzg/edit?usp=sharing)

    **id\_cliente:** Identificador de cliente. Un número entero de 1 a 5 dígitos asignado de forma exclusiva a cada cliente.

    **ano\_nacimiento:** Año de nacimiento del cliente.

    **nivel\_educacion:** Nivel de educación del cliente.

    **estado\_civil:** Estado civil del cliente.

    **ingreso**_**anual**_**dolar:** Ingresos anuales del hogar del cliente en dólares.

    **ninos**_**hasta**_**diez\_anos:** Número de niños pequeños hasta 10 años en el hogar del cliente.

    **ninos**_**mas**_**diez\_anos:** Número de niños con edad mayor a 10 años en el hogar del cliente.

    **fecha\_entrada:** Fecha de registro del cliente en la empresa.

    **respuesta\_campana:** Identifica si el cliente aceptó la campaña de marketing enviada. Donde 1 es sí y 0 es no.
*   [Tabla de transacciones](https://docs.google.com/spreadsheets/d/1dD2UF-XPWjPu7pkApGCQ1uIIVA0gAcZ-Qk4LPmxX10A/edit?usp=sharing)

    **id\_transaccion:** Identificador de transacciones. Un número entero de 9 dígitos asignado de forma exclusiva a cada transacción.

    **id\_cliente:** Identificador de cliente. Un número entero de 1 a 5 dígitos asignado de forma exclusiva a cada cliente.

    **fecha\_transaccion:** Fecha de compra en formato año-mes-día.

    **lugar\_transaccion:** El lugar donde se realizó la compra, puede ser en línea o en la tienda.
*   [Tabla resumen\_compras](https://docs.google.com/spreadsheets/d/1Tkg0lYsAiwu6CB6slktwUMdayWTvBq80SyX16r-xEVA/edit?usp=sharing)

    **id\_cliente:** Identificador de cliente. Un número entero de 1 a 5 dígitos asignado de forma exclusiva a cada cliente.

    **monto\_vino:** Valor monetario gastado en productos tipo vino.

    **monto\_frutas:** Valor monetario gastado en productos tipo fruta.

    **monto\_carnes:** Valor monetario gastado en productos tipo carne animal.

    **monto\_pescados:** Valor monetario gastado en productos tipo pescado.

    **monto\_dulces:** Valor monetario gastado en productos tipo dulces.

    **monto\_otros:** Valor monetario gastado en otros productos en general.

En la tabla de “clientes” que contiene la identificación (id_cliente) de cada cliente y sus características, la **identificación del cliente es única**, es decir, cada identificación (id_cliente) aparece una sola vez. La tabla de “transacciones” contiene el registro de compras que cada cliente realizó en el período de 2020-07-30 hasta 2022-06-29 y es esperable que haya más de una compra por cada cliente. Por último, en la tabla “resumen\_compras” encontramos el valor resumido que representa el total de compras realizadas por el cliente en este mismo periodo por categoría de producto.
