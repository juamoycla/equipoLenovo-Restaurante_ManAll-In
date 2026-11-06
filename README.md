# Descripción de la pyme

## 🍽️ Sobre ManAll-In

**ManAll-In** es una pyme de hostelería: un restaurante con servicio en sala, reservas y comida para llevar. Hoy trabaja de forma casi manual (agenda, boli y comandas que se cantan en cocina), lo que hace los trámites lentos y genera gastos ocultos.

🎯 **Objetivo:** digitalizar el negocio con carta QR, pedidos online, gestión de stock e IoT en cocina para atender mejor y reducir costes.

## Equipo y roles (PO, Scrum Master, Equipo de Desarrollo)

# 💻 Equipo Lenovo

| Rol | Integrante |
|---|---|
| 🎯 **Product Owner** | Raúl |
| 🧭 **Scrum Master** | Juan |
| 🛠️ **Equipo de desarrollo** | Gorka, Iván |


## 🏗️ Situación actual: arquitectura IT/OT (#2) + plano de la sala (#5)

### 🖥️ Clasificación IT
- 📦 Software de gestión de stock
- 🌐 Página web
- 🛵 Gestión de pedidos / para llevar

### ⚙️ Clasificación OT
- 📱 Carta QR
- 🍳 VLAN OT de cocina
- 🔌 VLAN Operativa


## Punto de dolor (#3)

## 🔥 Puntos de dolor (#3)

| Tipo | Problema | Detalle |
|---|---|---|
| 🎧 **Soporte** | Atención al cliente mejorable | No es mala, pero se puede agilizar con app y QR |
| ⏱️ **Productividad** | Herramientas ineficientes | Agenda y boli; hay que esperar a que se cante la comanda en cocina |
| 🔄 **Proceso** | Trámites lentos | — |
| 💸 **Financieros** | Gastos ocultos | — |

## Tecnologías habilitadoras: IoT, 5G, Blockchain, Robótica, RV/RA

 ## 1. Qué es y qué problema resuelve 
Es una tecnología que permite una rápida comunicación atraves de las tecnologías dentro del local 
 
## 2. Mejora que aporta 
Mejora muchísimo la experiencia del cliente y ayuda a la mejor comunicación entre tecnológias del local consumes 
 
## 3. ¿IT, OT o ambos? ¿Por qué? 
Es una mejora tanto IT como OT ya que si, mejora la conectividad, pero mejora todas las maquinarias del local 

 
## 4. Riesgo o límite 
El coste no es elevado, el de un router y una suscripción a una compañía de teléfono 

BLOKCHAIN
## 1. Qué es y qué problema resuelve 
Permite de forma automatizada llevar registro del inventario del local sin necesidad de contarlo a mano 

## 2. Mejora que aporta 
Mejora drásticamente la eficiencia a la hora de hacer inventario 

## 3. Nuevo servicio o mercado que abre 
Hace que sea más fácil saber cuándo hacer un pedido y que productos pedir 
 
## 4. ¿IT, OT o ambos? ¿Por qué? 
Es una mejora IT ya que se basa en controlador los datos de la empresa 
 
## 5. Riesgo o límite 
El coste no es bajo, ya que hay que digitalizar casi toda la forma de trabajar del restaurante y hay que explicar a los trabajadores como funciona

## ☁️ Cloud: dónde vive el sistema (#14)

### 🎯 Decisión inicial: modelo **SaaS** (Software as a Service)

En la primera fase, el sistema de ManAll-In funcionará con **soluciones SaaS** en la nube: herramientas ya hechas que se contratan por suscripción y se usan desde el navegador o una app, sin montar ni mantener servidores propios.

### 🤔 ¿Por qué SaaS y no IaaS / PaaS?

| Criterio | ☁️ SaaS | 🧱 PaaS | 🖥️ IaaS |
|---|---|---|---|
| 💸 **Coste inicial** | Bajo (cuota mensual) | Medio | Alto |
| 🛠️ **Mantenimiento** | Lo hace el proveedor | Compartido | Lo hacemos nosotros |
| ⏱️ **Puesta en marcha** | Días | Semanas | Meses |
| 👨‍💻 **Conocimientos técnicos** | Mínimos | Programación | Sistemas y redes |
| 📈 **Escalabilidad** | Cambiar de plan | Alta | Total |

### ✅ Justificación

- 🍽️ **Somos un restaurante, no una empresa de software.** El objetivo es servir mejor, no administrar servidores.
- 💸 **Atacamos los gastos ocultos (#3).** Pagamos una cuota fija y predecible, sin comprar hardware ni contratar a nadie de sistemas.
- ⚡ **Resultados inmediatos.** El TPV, la carta QR, los pedidos para llevar y el stock pueden funcionar en pocos días y sustituir enseguida la agenda y el boli.
- 👩‍🍳 **Fácil para el personal.** Son interfaces sencillas que ya se usan en otros restaurantes, así que hace falta poca formación.
- 🔒 **Seguridad y copias de seguridad incluidas.** El proveedor protege los datos de los clientes (reservas: nombre, correo y teléfono) y cumple el RGPD.
- 📱 **Acceso desde cualquier sitio.** Sala, cocina y gerencia ven la misma información en tiempo real desde la tablet o el móvil.

### 🧩 Ejemplos de SaaS a usar

- 🧾 **TPV y comandas:** pedidos que llegan directamente a la pantalla de cocina, sin tener que cantarlos.
- 📱 **Carta QR y pedidos online:** para llevar y pedidos desde la mesa.
- 📦 **Gestión de stock:** inventario e integración con proveedores.
- 📅 **Reservas:** gestión de mesas y clientes.
- 🌐 **Web:** creador de webs con hosting incluido.

### ⚠️ Riesgos y cómo los mitigamos

| Riesgo | Mitigación |
|---|---|
| 🔗 Dependencia del proveedor (*vendor lock-in*) | Elegir herramientas que permitan exportar los datos |
| 📶 Caída de Internet | Router 4G/5G de respaldo (ver IoT/5G) |
| 💰 Coste acumulado de suscripciones | Revisar los planes cada 6 meses |

## IA y mapa de datos (#12, #13)
Mapa Datos restaurante Man-All-In: 
Un mapa de datos es saber de dónde vienen los datos de una empresa y en cuales la empresa ha de ir con cuidado para cumplir el RGPD
En nuestro caso tenemos varios datos que tenemos sobre nuestros clientes sería solo en caso de que hagan una reserva: 
- Nombre 
- Correo Electrónico 
- Número de teléfono 
Los datos que más necesarios son y más vamos a manipular son acerca del inventario. Aquí contamos con todo lo que necesitamos para poder tenerlo automatizado: 
- Cuantos productos hay 
- Cuanto queda de cada producto 
- Numero de los proveedores 
- Cuanto necesitamos de cada producto para cada plato 
- Cuanto se ha gastado en cada día 
También contamos con datos acerca de la sostenibilidad del proyecto: 
- Gasto energético y de agua 

# Dos usos de IA para Man'All-In

## 1. Asistente de recomendación de platos

**Idea:** Cuando el cliente no sepa qué elegir de la carta, la IA le hará unas preguntas breves sobre:

- Qué ha comido en el día de hoy.
- Qué alimentos no le gustan.

Con esas respuestas, la IA le propondrá qué plato o platos de la carta elegir.

## 2. Control inteligente del stock de la nevera

**Idea:** La IA detecta qué alimentos se meten y se sacan de la nevera. Si un alimento se saca y no vuelve a meterse, o si detecta que queda poco, salta una alerta para reponerlo o comprar más porque se está acabando.

---

## Datos que se necesitan

| Propuesta | Dato o recurso necesario |
|---|---|
| **1. Recomendación de platos** | Hacer preguntas al cliente. |
| **2. Control de la nevera** | Una nevera inteligente **o** una cámara situada encima de la nevera, colocada de modo que tenga buena visibilidad. |
