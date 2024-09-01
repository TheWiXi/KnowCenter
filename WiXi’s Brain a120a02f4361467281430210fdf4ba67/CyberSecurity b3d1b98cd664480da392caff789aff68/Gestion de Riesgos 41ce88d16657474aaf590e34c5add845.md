# Gestion de Riesgos

## Gestión del riesgo

Un objetivo primordial de las empresas es proteger sus activos. Un **activo** es un elemento que se percibe como valioso para una organización. Este puede ser digital o físico. Ejemplos de activos digitales son la información personal de colaboradores/as, clientes o proveedores, como:

- Números de la Seguridad Social (SSN) o números únicos de identificación nacional asignados a personas.
- Fechas de nacimiento.
- Números de cuentas bancarias.
- Direcciones postales.

Ejemplos de activos físicos incluyen:

- Terminales de pago.
- Servidores.
- Computadoras de escritorio.
- Espacios de oficina.

Algunas estrategias habituales utilizadas para gestionar los riesgos son:

- **Aceptación**: aceptar un riesgo para evitar interrumpir la continuidad del negocio.
- **Prevención**: crear un plan para evitar el riesgo por completo.
- **Transferencia**: transferir el riesgo a un tercero para que lo gestione.
- **Mitigación**: disminuir el impacto de un riesgo conocido.

Además, las organizaciones aplican procesos de gestión de riesgos basados en marcos ampliamente aceptados para ayudar a proteger los activos digitales y físicos frente a diversas amenazas, riesgos y vulnerabilidades. Algunos ejemplos de estos son el Marco de Gestión de Riesgos ([RMF](https://csrc.nist.gov/projects/risk-management/about-rmf)) del Instituto Nacional de Estándares y Tecnología ([NIST](https://csrc.nist.gov/projects/risk-management/about-rmf)) y la Health Information Trust Alliance ([HITRUST](https://hitrustalliance.net/product-tool/hitrust-csf/?utm_term=&utm_campaign=HITRUST_i1_PaidSearch&utm_source=adwords&utm_medium=ppc&hsa_acc=2724012343&hsa_cam=16641331914&hsa_grp=136906352837&hsa_ad=598980848547&hsa_src=g&hsa_tgt=dsa-1659695676388&hsa_kw=&hsa_mt=&hsa_net=adwords&hsa_ver=3&gclid=Cj0KCQiAorKfBhC0ARIsAHDzsluRN5tSpCQal-rYnZLo2wUNppQdUHUba82LMX3JMGOoRPEJ6wG6-LgaAryYEALw_wcB)).

A continuación se indican algunos tipos comunes de amenazas, riesgos y vulnerabilidades que ayudarás a gestionar a las organizaciones desde tu rol como profesional de la ciberseguridad.

## Amenazas, riesgos y vulnerabilidades más comunes

### **Amenazas**

Una **amenaza** es cualquier circunstancia o evento que puede afectar negativamente a los activos. Como analista de ciberseguridad de nivel inicial, tu trabajo consiste en ayudar a preservar los activos de la organización frente a amenazas internas y externas. Por lo tanto, comprender cuáles son los tipos más comunes de amenazas es importante para tu trabajo. Las amenazas comunes incluyen:

- **Amenazas internas:** cuando miembros del personal o proveedores ****abusan de su acceso autorizado para obtener datos que pueden perjudicar a una organización.
- **Amenazas persistentes avanzadas (APT):** cuando agentes de amenaza mantienen el acceso no autorizado a un sistema durante un periodo prolongado de tiempo.

### **Riesgos**

Un **riesgo** es todo aquello que puede afectar la confidencialidad, integridad o disponibilidad de un activo. Una fórmula básica para determinar el nivel de riesgo es que este es igual a la probabilidad de una amenaza. Una forma de verlo es que un riesgo es llegar tarde al trabajo y las amenazas son el tráfico o un accidente que puedan ocasionar esa demora.

Existen diferentes factores que pueden afectar a la probabilidad de que se produzca un riesgo para los activos de una organización, entre ellos:

- **Riesgo externo:** se refiere a cualquier elemento, grupo o personas fuera de la organización que tienen el potencial de dañar sus activos, como agentes de amenaza que intentan acceder a información privada.
- **Riesgo interno:** se trata de colaboradores/as, proveedores externos o socios de confianza actuales o antiguos/as que pueden suponer un riesgo para la seguridad.
- **Sistemas heredados:** son sistemas antiguos que, si bien pueden no estar contabilizados o actualizados, aún pueden afectar a los activos, como estaciones de trabajo o sistemas de mainframe antiguos. Por ejemplo, una organización puede tener una máquina expendedora que acepta pagos con tarjeta de crédito o una estación de trabajo que todavía está conectada al sistema de contabilidad heredado.
- **Riesgo de múltiples partes:** hace referencia a que, el externalizar el trabajo a terceros, puede implicar darles acceso a propiedad intelectual, como información comercial confidencial, diseños de software y patentes.
- **Cumplimiento normativo/licencias de software:** tiene que ver con software que no está actualizado o no cumple la normativa, o parches que no se instalan a tiempo.

Hay muchos recursos, como el NIST, que proporcionan listas de [riesgos de ciberseguridad](https://www.nist.gov/itl/smallbusinesscyber/cybersecurity-basics/cybersecurity-risks). Además, el Open Web Application Security Project (OWASP) publica un documento estándar de concientización sobre los [10 riesgos de seguridad más críticos](https://owasp.org/www-project-top-ten/) para las aplicaciones web, que se actualiza regularmente.

**Nota:** La lista de tipos de ataques frecuentes de OWASP contiene tres nuevos riesgos para los años 2017 a 2021: diseño inseguro, fallas de integridad del software y los datos, y falsificación de solicitudes del lado del servidor. Esta actualización enfatiza el hecho de que la seguridad es un campo en constante evolución. También demuestra la importancia de mantenerse al día sobre las tácticas y técnicas usadas por los agentes de amenaza, para que puedas prepararte mejor para manejar este tipo de riesgos.

![image.png](Gestion%20de%20Riesgos%2041ce88d16657474aaf590e34c5add845/image.png)

### **Vulnerabilidades**

Una **vulnerabilidad** es una debilidad que puede ser aprovechada por una amenaza. Por lo tanto, las organizaciones deben inspeccionar periódicamente sus sistemas en busca de vulnerabilidades. Algunas de estas pueden ser:

- **ProxyLogon:** una vulnerabilidad preautenticada que afecta al servidor de Microsoft Exchange. Esto significa que un agente de amenaza puede completar un proceso de autenticación de usuario para implementar código malicioso desde una ubicación remota.
- **ZeroLogon:** una vulnerabilidad en el protocolo de autenticación Netlogon de Microsoft. Un protocolo de autenticación es una forma de verificar la identidad de una persona. Netlogon es un servicio que garantiza la identidad de un usuario antes de permitirle el acceso a la ubicación de un sitio web.
- **Log4Shell:** posibilita a los atacantes ejecutar código Java en la computadora de otra persona o filtrar información confidencial. Para ello, permite a un atacante remoto tomar el control de dispositivos conectados a Internet y ejecutar código malicioso.
- **PetitPotam:** afecta al gestor de redes de área local (LAN) de nueva tecnología de Windows (NTLM). Se trata de una técnica de robo que permite a un atacante basado en LAN iniciar una solicitud de autenticación.
- **Fallos de registro y supervisión de la seguridad:** capacidades de registro y supervisión insuficientes que dan lugar a que quienes perpetran un ataque aprovechen vulnerabilidades sin que la organización lo sepa.
- **Falsificación de solicitudes del lado del servidor:** permite a quienes perpetran un ataque manipular una aplicación del lado del servidor para que acceda a recursos backend y los actualice. También puede permitir que los agentes de amenaza roben datos.

Como analista de seguridad de nivel inicial, podrías encargarte de la gestión de vulnerabilidades, que consiste en monitorear un sistema para identificarlas y mitigarlas. Aunque existan parches y actualizaciones, si no se aplican, pueden producirse intrusiones. Por esta razón, el seguimiento constante es clave. Cuanto más temprano identifique una organización una vulnerabilidad y la aborde aplicando parches o actualizando sus sistemas, antes se podrá mitigar, reduciendo su exposición a la vulnerabilidad.

- Dominios de seguridad
    
    ## **Dominio 1: Seguridad y gestión de riesgos**
    
    **Todas las organizaciones deben desarrollar su postura de seguridad, es decir, su capacidad para gestionar la defensa de sus activos y datos críticos así como para reaccionar frente a los cambios. Algunos de los elementos del dominio de seguridad y gestión de riesgos que impactan en la postura de seguridad de una organización son:**
    
    - **Metas y objetivos de seguridad.**
    - **Procesos de mitigación de riesgos.**
    - **Cumplimiento normativo (compliance).**
    - **Planes para la continuidad del negocio.**
    - **Normativa.**
    - **Ética profesional y organizacional.**
    
    **La seguridad de la información, o InfoSec, también está relacionada con este dominio y se refiere a un conjunto de procesos establecidos para proteger la información. Una organización puede usar guías o manuales de estrategias (o procedimientos) e implementar la formación como parte de su programa de seguridad y gestión de riesgos, en función de sus necesidades y de los riesgos percibidos. Existen muchos procesos de diseño de InfoSec, como:**
    
    - **Respuesta a incidencias.**
    - **Gestión de las vulnerabilidades.**
    - **Seguridad en la aplicación.**
    - **Seguridad en la nube.**
    - **Seguridad de la infraestructura.**
    
    **Por ejemplo, un equipo de seguridad puede tener que modificar el tratamiento de la información de identificación personal (PII) para cumplir el Reglamento General de Protección de Datos (RGPD) de la Unión Europea.**
    
    ## **Dominio 2: Seguridad de los activos**
    
    **La seguridad de los activos implica gestionar los procesos de ciberseguridad de los activos organizacionales, lo cual incluye almacenamiento, mantenimiento, conservación y destrucción de datos físicos y virtuales. Dado que la pérdida o el robo de activos puede exponer a una compañía y aumentar el nivel de riesgo, es esencial hacer un seguimiento de los activos y los datos que contienen. Realizar un análisis del impacto en la seguridad, establecer un plan de recuperación y gestionar la exposición de los datos dependerá del nivel de riesgo asociado a cada activo. Las/los analistas de seguridad pueden necesitar almacenar, mantener y conservar datos mediante la creación de copias de seguridad, para asegurarse de poder restaurar el entorno en caso de que un incidente de seguridad ponga en riesgo los datos de la organización.**
    
    ## **Dominio 3: Arquitectura y diseño de seguridad**
    
    **Este dominio se enfoca en la gestión de la seguridad de los datos. Garantizar la existencia de herramientas, sistemas y procesos eficaces ayuda a proteger los activos y datos de una organización. Estos procesos son creados por quienes se dedican a la arquitectura e ingeniería de seguridad.**
    
    **Un aspecto importante de este dominio es el concepto de responsabilidad compartida, que implica que todas las personas involucradas asuman un papel activo en la reducción del riesgo durante el diseño de un sistema de seguridad. Los principios de diseño adicionales relacionados con este dominio, que se tratarán más adelante en el programa, son:**
    
    - **Simulación de amenazas.**
    - **Principio de privilegio mínimo.**
    - **Defensa en profundidad.**
    - **Fallar de forma segura.**
    - **Separación de funciones.**
    - **Simplicidad.**
    - **Confianza cero.**
    - **Confianza tras verificación.**
    
    **Un ejemplo de administración de datos es el uso de una herramienta de gestión de eventos e información de seguridad (SIEM) para monitorear los indicadores relacionados, ante un inicio de sesión o una actividad de usuario inusuales, que podrían indicar que un agente de amenaza está intentando acceder a datos privados.**
    
    ## **Dominio 4: Seguridad de las comunicaciones y de redes**
    
    **Este dominio se centra en la gestión y la seguridad de las redes físicas y las comunicaciones inalámbricas, incluidas las que son en el mismo lugar, remotas y en la nube.**
    
    **Las organizaciones que cuentan con entornos de trabajo remotos, híbridos y presenciales (en el lugar) deben asegurarse de que los datos permanezcan seguros y, a la vez, gestionar las conexiones externas y garantizar que quienes trabajan a distancia accedan de forma segura a las redes. Diseñar controles de seguridad de red, como el acceso restringido, puede ayudar a proteger a los/las usuarios/as y garantizar que la red de una empresa permanezca segura cuando sus empleados/as viajan o trabajan fuera de la oficina principal.**
    
    ## **Dominio 5: Gestión de identidades y accesos**
    
    **El dominio de gestión de identidades y accesos (IAM) se centra en mantener la seguridad de los datos, asegurándose de que las identidades de los/las usuarios/as sean confiables y estén autenticadas, y que el acceso a los activos físicos y lógicos esté autorizado. Esto ayuda a prevenir el acceso de usuarios/as no autorizados/as, al tiempo que permite que quienes están autorizados/as realicen sus tareas.**
    
    **Básicamente, el IAM utiliza lo que se conoce como el principio de privilegio mínimo, que es el concepto de otorgar solo el acceso y la autorización mínimos necesarios para completar una tarea. Por ejemplo, a un/a analista de ciberseguridad se le puede pedir que se asegure de que las/los representantes del servicio de atención al cliente solo puedan ver los datos privados de un/a cliente, como su número de teléfono, mientras trabajan en la resolución de un problema. Una vez resuelto el inconveniente, se deberá eliminar el acceso.**
    
    ## **Dominio 6: Evaluación y pruebas de seguridad**
    
    **El dominio de evaluación y pruebas de seguridad se enfoca en identificar y mitigar riesgos, amenazas y vulnerabilidades. Las evaluaciones de seguridad ayudan a las empresas a determinar si sus sistemas internos son seguros o están en riesgo. Las organizaciones pueden emplear pruebas de penetración, un proceso conocido como pentesting, para encontrar vulnerabilidades que podría aprovechar un agente de amenaza.**
    
    **Este dominio sugiere que las organizaciones realicen pruebas de control de la seguridad, y que recopilen y analicen datos. Además, se enfatiza la importancia de realizar auditorías de seguridad para monitorear y reducir la probabilidad de que se produzca una filtración de datos. Para contribuir a este tipo de tareas, las y los profesionales de la ciberseguridad pueden encargarse de auditar los permisos de usuarios/as, a fin de confirmar si tienen los niveles correctos de acceso a los sistemas internos.**
    
    ## **Dominio 7: Operaciones de seguridad**
    
    **El dominio de operaciones de seguridad se centra en la investigación de una posible filtración de datos y la implementación de medidas preventivas después de que se haya producido un incidente. Esto incluye el uso de estrategias, procesos y herramientas como:**
    
    - **Entrenamiento y concientización.**
    - **Informes y documentación.**
    - **Detección y prevención de intrusiones.**
    - **Herramientas SIEM.**
    - **Gestión de registros.**
    - **Gestión de incidentes.**
    - **Manuales de estrategias (playbooks).**
    - **Análisis forense posterior a una filtración.**
    - **Reflexión sobre las lecciones aprendidas.**
    
    **Los y las profesionales de ciberseguridad involucrados/as en este dominio trabajan en equipo para gestionar, prevenir e investigar amenazas, riesgos y vulnerabilidades. Están entrenados/as para hacer frente a ataques activos, como el acceso a grandes cantidades de datos desde la red interna de una organización, fuera del horario normal de trabajo. Una vez identificada una amenaza, el equipo trabaja para mantener a salvo los datos y la información privada.**
    
    ## **Dominio 8: Seguridad en el desarrollo de software**
    
    **El dominio de seguridad en el desarrollo de software se enfoca en el uso de prácticas y políticas de programación para crear aplicaciones seguras. Contar con ellas ayuda a ofrecer servicios seguros y fiables, y a proteger a las organizaciones y sus usuarios/as.**
    
    **La seguridad debe incorporarse en cada elemento del ciclo de vida del desarrollo de software, desde el diseño y el desarrollo hasta las pruebas y el lanzamiento. Para lograr la seguridad efectiva, es necesario tener en mente la seguridad en cada paso del proceso de desarrollo de software. No se la puede considerar como un aspecto secundario o posterior.**
    
    **Realizar pruebas de seguridad de las aplicaciones puede ayudar a garantizar que las vulnerabilidades sean identificadas y mitigadas adecuadamente. Además, es necesario disponer de un sistema que permita evaluar las convenciones de programación, los ejecutables de software y las medidas de seguridad incorporadas en el mismo. También, es clave contar con profesionales de control de calidad y de pruebas de penetración que se encarguen de verificar que el software cumpla con los estándares de seguridad y rendimiento establecidos. Por ejemplo, un/a analista de nivel inicial que trabaje para una empresa farmacéutica podría tener la responsabilidad de asegurarse de que el cifrado, o encriptación, esté configurado correctamente en un nuevo dispositivo médico que almacenará datos privados de pacientes.**
    
- Amenazas, riesgos y vulnerabilidades
    - Ingenieria social Aprovecharse del error humano
    * Fishing
- Capas de la Red
    - web
    - Deep Web (suele requerir autorizacion para acceder a ella)
    - Dark Web (se accede con software especifico)
- **Marco de Gestión de Riesgos (RMF) (Framework)**
    - Preparar: Actividades necesarias para gestionar los riesgos de seguridad y privacidad
    - Categorizar: Desarrollar porcesos y tareas de manejo de riesgos
    - Seleccionar: Elegir, personalizar y capturar la documentacion de los controles que protegen a una organizacion
    - Implementar: implementar planes de seguridad y privacidad
    - Evaluar: determinar si los controles establecidos se implementan correctamente o si cumplen con los requerimientos
    - Autorizar: Ser responsables de los riesgos y vulnerabilidades que existen
    - Monitorear: Estar al tanto de como operan los sistemas evaluear y mantener las operaciones tecnicas
- Marcos y Controles
    
    **Cómo se vinculan los marcos y los controles**
    
    Anteriormente, viste de qué modo las organizaciones usan marcos y controles de seguridad para protegerse contra amenazas, riesgos y vulnerabilidades. Esto incluye debates sobre el Marco de Gestión de Riesgos (RMF) y el Marco de Ciberseguridad (CSF) del Instituto Nacional de Estándares y Tecnología (NIST), así como la tríada de confidencialidad, integridad y disponibilidad (CID). En esta lección, aprenderás un poco más sobre los marcos y controles de seguridad cibernética y cómo se pueden combinar para mitigar los riesgos empresariales.
    
    **Marcos y controles**
    
    Los **marcos de seguridad** son pautas utilizadas para elaborar planes que ayuden a mitigar los riesgos y las amenazas a los datos y la privacidad. Estos marcos brindan soporte a las organizaciones para acatar las leyes y las normas de cumplimiento. Por ejemplo, en el sector de la salud se utilizan marcos para cumplir con la Ley de Transferencia y Responsabilidad de los Seguros Médicos (HIPAA) de los Estados Unidos, que exige a profesionales médicos mantener a resguardo la información de sus pacientes.
    
    Los **controles de seguridad**, en tanto, son medidas de protección diseñadas para reducir riesgos de seguridad *específicos*. Estas medidas son utilizadas por las organizaciones para disminuir los riesgos y amenazas a los datos y la privacidad. Por ejemplo, una medida de control que se puede usar junto con los marcos de seguridad para garantizar que el cumplimiento de HIPAA en un hospital es requerir que las y los pacientes utilicen autenticación de múltiples factores (MFA) para acceder a sus registros médicos. El uso de una medida como la MFA para validar la identidad de las personas es una manera de ayudar a mitigar posibles riesgos y amenazas a la seguridad de los datos privados.
    
    **Marcos y controles específicos**
    
    Existen diversos marcos y controles que las organizaciones pueden utilizar para cumplir con las regulaciones y alcanzar sus objetivos de seguridad. Los marcos abordados en esta lección son el Marco de Amenaza Cibernética (Cyber Threat Framework, CTF) y la Organización Internacional de Normalización/Comisión Electrotécnica Internacional (ISO/IEC) 27001. También se explican varios controles de seguridad comunes, que se usan junto con este tipo de marcos.
    
    **Marco de Amenaza Cibernética (Cyber Threat Framework, CTF)**
    
    De acuerdo con la Oficina del Director de Inteligencia Nacional, el CTF fue desarrollado por el gobierno de los Estados Unidos con el fin de proporcionar “un lenguaje común para describir y comunicar información sobre la actividad de amenazas cibernéticas”. Al ofrecer un lenguaje común, el CTF ayuda a las y los profesionales de ciberseguridad a analizar y compartir información de manera más eficiente. Esto permite a las organizaciones mejorar su respuesta, dado que las tácticas y técnicas de los agentes de amenaza son múltiples y, por lo tanto, la ciberseguridad está en constante evolución.
    
    **Organización Internacional de Normalización/Comisión Electrotécnica Internacional (ISO/IEC) 27001**
    
    Un marco reconocido internacionalmente y muy utilizado es el ISO/IEC 27001. El conjunto de normas ISO 27000 permite a las organizaciones de todos los sectores y tamaños gestionar la seguridad de sus activos, como la información financiera, la propiedad intelectual, los datos del personal y la información confiada a terceros. Este marco establece los requisitos para un sistema de gestión de seguridad de la información, las prácticas recomendadas y los controles que respaldan la capacidad de una organización para gestionar los riesgos. Si bien el marco ISO/IEC 27001 no exige el uso de controles específicos, proporciona una serie de controles que las empresas pueden utilizar para mejorar su postura de seguridad.
    
    ### **Controles**
    
    Los controles se utilizan junto con los marcos para reducir la posibilidad y el impacto de una amenaza, riesgo o vulnerabilidad de seguridad. Estos pueden ser físicos, técnicos y administrativos, y se utilizan típicamente para prevenir, detectar o corregir problemas de seguridad.
    
    Ejemplos de controles físicos:
    
    - Puertas, barreras y cerraduras
    - Guardias de seguridad
    - Vigilancia por circuito cerrado de televisión (CCTV), cámaras y detectores de movimiento
    - Tarjetas de acceso o credenciales para ingresar a los espacios de la oficina
    
    Ejemplos de controles técnicos:
    
    - Cortafuegos (firewalls)
    - Autenticación de múltiples factores (MFA)
    - Software de antivirus
    
    Ejemplos de controles administrativos:
    
    - Separación de funciones
    - Autorización
    - Clasificación de activos
    
    Para obtener más información sobre los controles, especialmente aquellos utilizados para proteger activos relacionados con la salud de diversos tipos de amenazas, consulta la [presentación sobre Control de Acceso Físico](https://www.hhs.gov/sites/default/files/physical-access-control.pdf) del Departamento de Salud y Servicios Humanos de los Estados Unidos.
    
- Triada CID
    
    # Usa la tríada CID para proteger a las organizaciones
    
    Anteriormente, te presentamos la tríada de confidencialidad, integridad y disponibilidad (CID) y de qué modo ayuda a las organizaciones a evaluar y mitigar el riesgo. En esta lección, aprenderás cómo los/as analistas de ciberseguridad la utilizan en el entorno laboral.
    
    ## Tríada CID para analistas
    
    La **tríada CID** es una guía que ayuda a las organizaciones a evaluar los riesgos y establecer sistemas y políticas de seguridad. Está compuesta por tres elementos fundamentales: confidencialidad, integridad y disponibilidad. Las/los analistas de ciberseguridad trabajan en mantener estos elementos para asegurar un nivel de riesgo aceptable. Diseñar sistemas y políticas con estos elementos en mente ayuda a establecer una **postura de seguridad** exitosa. La postura de seguridad se refiere a la capacidad que tiene una organización para gestionar la defensa de sus activos y datos críticos, así como de reaccionar ante los cambios de manera efectiva.
    
    ### **Confidencialidad**
    
    La **confidencialidad** refiere a que solo los/las usuarios/as autorizados/as pueden acceder a activos o datos específicos. En una organización, la confidencialidad puede mejorarse mediante la implementación de principios de diseño, como el principio de mínimo privilegio, que limita el acceso de las personas solo a la información que necesitan para llevar a cabo las tareas laborales. Limitar el acceso es una forma de mantener la confidencialidad y la seguridad de los datos privados.
    
    ### **Integridad**
    
    La **integridad** implica que los datos son verificables, auténticos y confiables. Es esencial contar con protocolos para verificar la autenticidad de los datos y una manera de hacerlo es mediante la [criptografía](https://www.nist.gov/cryptography#:~:text=Cryptography%20uses%20mathematical%20techniques%20to,that%20drives%20research%20and%20innovation.), que se utiliza para transformar los datos, para que las partes no autorizadas no puedan leerlos ni manipularlos (NIST, 2022). Otro ejemplo de cómo una organización podría implementar la integridad es mediante la activación del cifrado, que es el proceso de convertir los datos de un formato legible a uno codificado. Se puede utilizar para evitar el acceso a información, como los mensajes en la plataforma de chat interna de una organización.
    
    ### **Disponibilidad**
    
    La **disponibilidad** refiere a que los datos son accesibles para aquellas personas autorizadas a usarlos. Cuando un sistema cumple tanto los principios de disponibilidad como los de confidencialidad, los datos pueden ser utilizados cuando sea necesario. En el entorno laboral, esto puede significar que la organización permite al personal que trabaja de forma remota acceder a su red interna para desempeñar sus tareas laborales. Es importante tener en cuenta que el acceso a los datos en la red interna sigue siendo limitado, según el tipo de acceso que los/las empleados/as necesiten para realizar su trabajo. Si, por ejemplo, una persona trabaja en el departamento de Contabilidad de la empresa, es posible que necesite acceso a las cuentas corporativas, pero no a los datos relacionados con proyectos que estén desarrollando en ese momento.