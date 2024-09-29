# Aplicación web para una integración estable entre ZOHO y NOTION, pertenecientes a la empresa DOSPORDOS GRUPO IMAGEN S.L.

Esta aplicación contiene una API que está integrada con **ZOHO Y NOTION** para la empresa **DOSPORDOS GRUPO IMAGEN S.L.**. Su propósito es administrar la integración de los datos de ambas aplicaciones, a través de webhooks, workflows, funciones Delug y sincronizadores.

Así mismo se está teniendo una curva de aprendizaje y experimentando, para servir archivos estáticos y dimámicos a través de la aplicación.

## Características
- Integración con **ZOHO**.
- Integración con **NOTION**.
- Gestión de datos y sincronizaciones.

La documentación de la API está en construcción.

Instalar las dependecias del archivo package.json con npm o yarn.

Actualmente la aplicación es servida por Apache, el cual funciona como un proxy inverso, tener en cuenta las siguientes notas si se desea crear un entorno similar usando xampp:

**PASOS PARA SERVIDOR XAMPP EN ENTORNO DE DESARROLLO Y APACHE EN ENTORNO DE PRODUCCIÓN:**
- Se instala node js, se instala express, se instala pm2, se instala dotenv.
- Se configura apache para servir como proxy inverso.
- Se crea dos virtual host en apache, uno para localhost y sus carpetas en php, otro que apunte al proyecto en nodejs... Siempre en el servidor real se crearán virtual hosts para cada proyecto pues irá asociado a un dominio.
- Se crea los host en windows para la asignación de dominios, en la ruta aproximada de system32/drivers/etc/host.
- Se configura el servidor del proyecto nodejs para poder servir archivos estáticos y módulos de la aplicación.
- Se debe asociar los certificados https tanto en express como en apache.