# Introducción a la Ciberseguridad
- **¿Qué es la ciberseguridad?**
- **Importancia de la ciberseguridad**
- **Beneficios de la ciberseguridad**
- **Retos de la ciberseguridad**
- **Entiende tus riesgos**

## Campos de acción de la ciberseguridad
- **Seguridad de la información**
- **Seguridad de aplicaciones**
- **Seguridad en redes**
- **Seguridad en la nube**
- **Seguridad física**
- **Cultura en ciberseguridad**

## Ciberamenazas
### Malware
Software malicioso creado para causar daño que afecta todo tipo de dispositivos y sistemas operativos.

**¿Qué puede hacer?**
- Crackear contraseñas y acceder a sistemas críticos vía shell.
- Replicarse en la red (VLAN).
- Afectar la operatividad de sistemas vitales para la empresa.
- Realizar **cryptojacking**, utilizando el procesamiento para minería de criptomonedas.
- Secuestrar datos, alterando la integridad de la información.
- Controlar equipos remotamente para generar ciberataques dirigidos (**zombies**).

**Tipos de Malware**
- **Virus**: Modifica programas para difundirse.
- **Ransomware**: Cifra archivos y cobra rescate.
- **Spyware**: Accede a contraseñas, registros de teclado, etc.
- **Bots**: Ejecutan ciberataques dirigidos.

**Verificar Malware**
- [VirusTotal](https://www.virustotal.com/gui/home/upload)
- [Hybrid Analysis](https://www.hybrid-analysis.com/)

### Ransomware
Utiliza técnicas de cifrado robusto y es lucrativo para ciberdelincuentes, dirigido casi siempre a empresas.

**Factores de Riesgo**
- Direcciones IP públicas sin auditar.
- Ausencia o mala configuración del firewall.
- Falta de protección en endpoints.
- Carencia de prácticas de **hardening**.
- Débil cultura de seguridad.

**Cibercontroles**
- Educar a todos los equipos.
- Asegurar todos los activos de información.
- Respaldar información crítica.
- Nunca pagar rescates.

**Recursos**
- [No More Ransom](https://www.nomoreransom.org/en/index.html)
- [PCMag Ransomware Protection](https://www.pcmag.com/picks/the-best-ransomware-protection)

### Ingeniería Social
Interacciones y técnicas utilizadas para manipular psicológicamente a las víctimas.

**Ciclo de Vida**
1. **Investigación**: Identificación, captura de información y definición del método de ataque.
2. **Ejecución**: Realización del ataque y obtención de información.
3. **Cierre**: Terminación de interacción y eliminación de evidencias.

**Cibercontroles**
- Validar el origen de correos o contactos.
- Utilizar **2FA** o **MFA**.
- Promover la cultura de ciberseguridad.

### Phishing
Técnica para robar datos personales y financieros mediante suplantación de identidad.

**Técnicas de Phishing**
- **Email Scams**: Envío masivo de correos falsos.
- **Spear Phishing**: Ataques dirigidos con conocimiento previo organizacional.

**Cibercontroles**
- **Security Education** con herramientas como [GoPhish](https://getgophish.com/).
- Fortalecer cuentas con **2FA** o **MFA**.
- Denunciar enlaces sospechosos.

### Denegación de Servicios (DoS)
Ataques que afectan la disponibilidad tecnológica por saturación de tráfico.

**Tipos**
- **Basados en volumen**: Saturan el ancho de banda (UDP, ICMP).
- **De protocolo**: Consumen recursos del servidor (SYN, Ping of Death).
- **Capa de aplicación**: Solicitudes masivas hasta colapsar servicios.

**Cibercontroles**
- Adquirir soluciones de seguridad como servicio.
- Aplicar **hardening** y evitar configuraciones por defecto.

### Man-in-the-Middle (MitM)
Ataques que interceptan comunicaciones para capturar información sensible.

**Tipos**
- **IP Spoofing**: Alteración de headers para suplantar direcciones IP.
- **ARP Spoofing**: Enlace entre direcciones MAC e IP legítimas.
- **DNS Spoofing**: Modificación de registros DNS.

**Cibercontroles**
- No omitir alertas de navegadores.
- Cerrar sesiones cuando no se usen aplicaciones.
- Usar **VPN** y cifrar comunicaciones (TLS 1.3+).

## Controles en ciberseguridad
### Gestión de accesos
Tratamiento de credenciales, tokens y recursos de autenticación.

**Clasificación**
- **Locales (Offline)**: Administración local (e.g., KeePass).
- **Servicios web (Online)**: Sincronización en la nube (e.g., 1Password).
- **Basados en token**: Autenticación con hardware (e.g., USB).

**Beneficios**
- Cifrado de repositorios.
- Generación de contraseñas robustas.
- Opciones sin contraseña (passwordless).

### Firewall
Dispositivo que monitorea y controla el tráfico de red bajo reglas de seguridad.

**Implementaciones**
- **On-premise**: Hardware dedicado.
- **Cloud**: Soluciones modulares y escalables.

**Beneficios**
- Panorama de seguridad.
- Calidad del servicio (**QoS**).
- Bloqueo de amenazas emergentes.

**Recursos**
- [Cómo elegir un firewall](https://www.itsasap.com/blog/how-to-choose-a-firewall)

### IPS/IDS (Intrusion Prevention/Detection Systems)
- **IDS (Sistema de Deteción de Intrusos)**: Es una herramienta de seguridad de red que analiza el tráfico interno para detectar actividad maliciosa y alertar al administrador del sistema.
- **IPS (Sistema de Prevención de Intrusos)**: Es la evolución de los IDS. Este, además de alertar al administrador del sistema cuando detecta actividad maliciosa; puede bloquear, capturar o eliminar paquetes maliciosos.

**Clasificación**
- **NIPS (Network Intrusion Prevention)**: Basado en la red.
- **HIPS (Host Intrusion Prevention System)**: Basado en el host.
- **WIPS (Wireless Intrusion Prevention System)**: Escanea redes WiFi.

**Beneficios**
- Integración con otras soluciones.
- Mayor eficiencia en otros controles de seguridad.
- Ahorro de Tiempo.
- Compliance.
- Personalizable.

### Correlación y Gestión de Eventos (SIEM)
Administración de eventos e información de seguridad. Es un campo de la seguridad
informática del que surgen soluciones que centralizan todas las fuentes de información para
así tener una visión mas completa de posibles amenazas, cumplimiento y manejo de incidentes.

**¿Como funciona?**
- Gestión de registros.
- Correlación de eventos y análisis.
- Monitoreo de incidentes y alertas de seguridad.
- Gestión de compliance e informes.

**Capacidades**
- Agregación de Información
- Correlación
- Alerta
- Dashboard
- Compliance
- Retención
- Análisis Forense

**¿Por qué es importante?**
- Puede ayudar a detectar zero-days.
- Normalización y categorización de logs.
- Visualización de eventos.
- Detección de malas configuraciones.
- Puede detectar comunicaciones maliciosas y canales de encriptados.

### Copias de Seguridad
Son copias de la información original almacenadas en distintos medios y que pueden ser usadas
para recuperar la información en caso de su pérdida.

**¿Por qué se puede perder la información?**
- Desastre natural
- Eliminación accidental
- Robo
- Corrupción de información
- Virus informático

**Métodos**
- Copia completa/espejo
- Copia incremetal
- Copia en tiempo real (CDP)

**Medios**
- Cinta magnética
- Medios ópticos
- Discos duro tradicional (HDD)
- Discos duro en estado sólido (SDD)
- Servicio remoto (cloud)

**Consideraciones**
- Redundancia/replicación de las copias de seguridad
- Cifrado de los datos
- Refactorización
- Compresión
- Limpieza automática de datos
- Seguridad de las copias de seguridad
- Periodo de retención de la información
- Validación de integridad
- Monitoreo

**Conceptos Clave**
- **Punto Objetivo de Recuperación (RPO)** Periodo objetico máximo del que se puede tolerar pérdida de información
- **Tiempo Objetivo de Recuperación (RTO)** Cantidad de tiempo entre un desastre y la Recuperación de las funciones de negocio

### Cifrado y Descifrado
- **Cifrado:** Es el proces de convertir información a un formatp ilegible mediante el uso de una llave definida y procesos matemáticos
con el fin de proteger la **confidencialidad** de la misma.
- **Descifrado:** Es el proceso de revertir la información a su formato original mendiante el
uso de una llave para que pueda ser usada normalmente de nuevo.

**Tipos de Cifrado**
- **Cifrado Simétrico:** Se usa la misma llave para cifrar y para descifrar
- **Cifrado Asimétrico:** Se tienen dos llaves. Llave pública (k+) y llave privada (k-)
lo que se cifra con una llave pública solo puede ser descifrado con la llave privada correspondiente
y viceversa.

**Cifrado en dispositivos personales**
Si pierdes o te roban tu computador o celular, tus archivos estarán pretegidis si el disco duro estaba cifrado.

### VPN (Virtual Private Network)
Es una tecnologia que permite la conexión de un usuario a la red publica (internet) como si estuviera en una red privada (intranet empresarial) al tiempo que cifra toda la información enviada.

**¿Como funciona?**
Toda la actividad se cifra y pasa por un intermediario (servidor VPN) el cual reenvia y recibe las peticiones a otros sitios o servicios web.

**¿Por qué debo usar una?**
- Si la empresa tiene aplicaciones que solo pueden ser accedidas desde su red interna.
- Cifrar datos enviados en redes no confiables.
- Ocultar datos enviados en redes no confiables.

### Endpoint Protection
Es la práctica de proteger todos los dispositivos finales de una red (computadores, celulares, IoT, etc.) mediante la integración de varias herramientas y soluciones. 
Es la siguiente iteración de las soluciones de antivirus tradicionales que se basaban
en firmas digitales.

**Características**
- Clasificación con Machine Learning.
- Protección avanzada de múltiples dispositivos.
- Protección de navegación web.
- Data Lost Protection. DLP
- Firewall Integrado.
- Bloqueo de Phishing y Ataques por Correo.
- Protección de Amenazas Internas.
- Vista Centralizada de Todos los Dispositivos
- Cifrado de datos.

### BCP (Plan de Continuidad de Negocio)
"Continuidad de negocio" Es la capacidad de una organización de continuar operando y entregando productos y/o servicios
según unos niveles predefinidos aceptables luego de un incidente disruptivo.

BCP es un documento que cotiene toda la información necesaria para lograr la "continuidad de negocio".
Recopila el resultado de un proceso completo que incluye, entre otras cosas, los siguiesntes pasos:

**Identificar:**
1. Principales funciones de negocio
2. RTO y RPO por función de negocio
3. Recursos requeridos por función de negocio
4. Impacto/costo financiero
5. Impacto/costo operacional
6. Impacto/costo legal

**Análisis de Riesgos**
1. Se busca identificar amenazas, vulnerabilidades y riesgos de la información.
2. Por cada amenaza identificada se considera su probabilidad y el impacto.
3. Las amenazas se pueden clasificar en naturales, causadas por el hombre o fallas de infraestructura.
4. Se pueden identificar controles y costos para cada riesgo.

**Plan de Recuperación**
Desarrollar una guía que permita al negocio volver a un nivel de opración aceptable.
Esta guía debe contar con:
1. Eventos que desencadenan el plan.
2. Equipo responsable de atención de incidentes.
3. Plan de recuperación de incidentes.
4. Lista de contactos.

**Plan de Recuperación de Desastres (DRP)**
Este incluye:
1. Inventario de infraestructura vital.
2. Manual de procedimientos para restablecimiento.
3. Operaciones manuales para reemplazar sistemas temporalmente.

**Prueba y Mantenimiento**
Se deben establecer estrategias para:
1. Probar la efectividad del plan regularmente.
2. Entrenar al personal para que conozcan el plan.
3. Actualizar el plan continuamente.

### Data Loss Prevention (DLP)
Una solución que detecta y previene fugas de información. Detecta y bloquea la extracción de información
en uso (dispositivos), en movimiento (red) y almacenada (discos).

**¿Por qué es necesario?**
1. Previene fugas de información.
2. Protege información sensitiva personal (PII)
3. Progete propiedad intelectual (IP)
4. Ayuda al cumplimiento de regulaciones como CCPA, GDPR, HIPAA, entre otros.

### Gestión de Incidentes de Ciberseguridad
Es un proceso de permite una respuesta efectiva y rápida a ciberataques. Idealmente,
existe un plan que documenta una serie de procesos y pasos que se deben realizar en 
cada fase de la respuesta a un incidente. NIST 800-61.

**¿Cómo responder ante un incidente de seguridad?**
1. Preparación: Estimamos las necesidades y establecemos procedimientos.
2. Detección y Análisis: Es identificar los signos inusuales que pueden generar dicho incidente.
3. Identificación: Identificamos que tipo de incidente fue y ocurrió, que tan grave puede ser.
4. Notificación: Reportamos, notificamos y registramos el incidente.
5. Clasificación y Priorización: Debemos determinar el tipo de incidente, clasificarlo y así
saber qué tan grave es y qué tanto nos puede afectar.
6. Contención, Resolución y Recuperación: Detenemos el ataque y evitar que se propague. Resolvemos
el incidente. Recuperamos los datos.
7. Acciones Posteriores Al Cierre: Lecciones aprendidas. Identificamos las causas del incidente,
por qué pasó y cómo podemos hacer, para qué no vuelva a pasar.


## Roles en ciberseguridad
- **CEO (Chief Executive Officer)**
- **CISO (Chief Information Security Officer)**
- **CSO (Chief Security Officer)**
- **CIO (Chief Information Officer)**
- **Penetration Testers** (Red Team, Blue Team)
- **Stakeholders**
