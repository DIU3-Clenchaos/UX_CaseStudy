## DIU - Practica2, entregables

### Ideación 
Para realizar el apartado de ideación, nuestro equipo de investigadores y diseñadores UX han decidido realizar un mapa de empatía, en el que recopilaremos la información que rodea a un usuario, con objetivo de obtener puntos fuertes, débiles y llevar a cabo mejoras.

### Mapa de empatía
<img width="9362" height="3689" alt="Empathy Map" src="https://github.com/user-attachments/assets/2ade4ee3-7068-4186-80ba-aefc866d7a8f" />

### PROPUESTA DE VALOR
Nuestro propósito con el sitio de The Champions Burguer se enfoca sobre todo en un sistema de mapa interactivo del recinto en el que se celebra la competición, con el objetivo de que les sirva a los usuarios para
poder decidir si pedir a domicilio o ir presencialmente dependiendo de la cantidad de personas que haya y el tiempo estimado de cola en los foodtrucks. Pensamos que es algo sumamente importante en un evento
como este, pues la mayoría de personas asiste sin esperarse un aforo tan extremo. De esta forma, podrán anticiparse al estado de los foodtrucks en todo momento.

También proponemos la implementación de un sistema para reservar mesas y asientos del evento. Así, los clientes pueden asegurarse un lugar en el que comer sentados de manera dinámica y sencilla.

Por último, hemos pensado en las personas con intolerancias o alergias y optamos por añadir un filtro de alérgenos que permita al cliente ver solo aquellas hamburguesas que cumplan con sus necesidades, ofreciendo
seguridad y confianza al usuario.

### TASK ANALYSIS<img width="1920" height="1080" alt="Scope Canvas (2)" src="https://github.com/user-attachments/assets/fb8b8a7e-ebcb-4604-b4d1-2a5f2d913f22" />


# User Task Matrix: Remake Champions Burger
Para la realización de nuestra matriz de tareas, hemos decidido recopilar aquellas funcionalidades mas importantes y necesarias para el usuario, de manera que estableceremos 3 tipos de prioridades segun la importancia de uso para el usuario. 
A continuación se presenta la matriz cruzando las tareas principales (extraídas del Task Analysis) con los perfiles de usuario identificados.

| Tarea / Acción | 🚶‍♂️ Asistente Presencial | 🛵 Cliente Delivery / Takeaway | 🥗 Usuario con Alergias / Dietas |
| :--- | :---: | :---: | :---: |
| **Usar mapa interactivo (ver food trucks, colas y POIs)** | Alta | N/A | Media |
| **Consultar carta y precios de las hamburguesas** | Alta | Alta | Alta |
| **Consultar y filtrar por alérgenos** | Baja | Baja | Alta |
| **Realizar pedido a domicilio / Takeaway** | N/A | Alta | Media |
| **Reservar asientos en el recinto** | Alta | N/A | Media |

---

## 💡 Notas sobre los perfiles

* **Asistente Presencial:** Es el usuario que va físicamente al evento. Su prioridad es no hacer cola (usar el mapa) y encontrar sitio para sentarse.
* **Cliente Delivery/Takeaway:** No le importa el mapa ni las colas del recinto; solo quiere ver el menú, los precios y pedir su hamburguesa para comerla en otro lado.
* **Usuario con Alergias / Dietas Especiales:** Perfil destacado (basado en la métrica de "% de pedidos que filtran alérgenos"). Su tarea crítica es consultar ingredientes antes de realizar cualquier otra acción.
  


### ARQUITECTURA DE INFORMACIÓN

* Sitemap
<img width="1151" height="751" alt="sitemap (3)" src="https://github.com/user-attachments/assets/9bd56aea-a7c4-4a23-950e-721138ff0025" />





* Labelling
  
| Web                       | Información                                                                 | Referencia |
|--------------------------|----------------------------------------------------------------------------|------------|
| Página de Inicio         | Página inicial de la Web                                                   | 🏠         |
| Carta                    | Catálogo completo de la oferta gastronómica                                | 📖         |
| Participantes            | Información sobre los participantes                                        | 🚙         |
| Filtros                  | Herramienta para afinar la búsqueda en el menú                             | 🔍         |
| Hamburguesas             | Catálogo detallado con fotos, ingredientes y precios de cada hamburguesa  | 🍔         |
| Carrito                  | Resumen de los productos seleccionados antes de comprar                   | 🛒         |
| Pago                     | Información y gestión de pagos                                             | 💵         |
| Mapa Interactivo         | Plano digital del recinto para los asistentes                              | 🗺         |
| Reservas                 | Sistema para asegurar un sitio antes de asistir                           | ✍         |
| Selección de Mesas       | Mapa visual para elegir mesa o zona                                       | 🪑         |
| Horarios                 | Selector de tramos horarios disponibles                                   | 📅         |
| Confirmación de Reservas | Genera ticket o código QR para acceder a la mesa                          | ✅         |
| FAQs                     | Preguntas frecuentes para resolver dudas rápidas                          | ❓         |
| Contacto                 | Información y vías de comunicación con la organización                    | 📮         |


### Prototipo Lo-FI Wireframe 


<img width="1440" height="1440" alt="index" src="https://github.com/user-attachments/assets/8e55df92-376c-4d41-966e-b8eaac2d0034" />


<img width="1440" height="1440" alt="carta" src="https://github.com/user-attachments/assets/aa613317-1f18-451a-b702-3278afd1be1d" />


<img width="1440" height="1440" alt="mapa_interactivo" src="https://github.com/user-attachments/assets/d4a94a74-6ee8-4174-af20-7046ff5ebf81" />


<img width="1440" height="1440" alt="reservas" src="https://github.com/user-attachments/assets/0d5397a4-cb19-4562-b623-650b8a254bfa" />


### Conclusiones  
Tras el análisis exhaustivo de la plataforma actual y el desarrollo de nuestra propuesta de diseño, hemos llegado a las siguientes conclusiones:
*Identificación de puntos críticos: La web oficial presenta carencias en la gestión de flujos de usuarios en eventos masivos. La falta de información en tiempo real sobre esperas y ocupación genera una fricción innecesaria que hemos resuelto mediante el mapa interactivo dinámico.
*Optimización de la Arquitectura: El diseño del nuevo sitemap no solo organiza el contenido, sino que prioriza la conversión. Hemos simplificado el camino del usuario (user journey) para que el paso de "ver una hamburguesa" a "realizar el pedido" sea directo e intuitivo.
*Validación del Wireframe: La creación de los wireframes nos ha permitido validar que la sencillez visual es compatible con la funcionalidad avanzada (filtros de alérgenos y reservas). Hemos pasado de una web puramente informativa a una herramienta logística para el asistente.

La realización de esta práctica ha sido fundamental para entender que el diseño UX/UI no se limita a la estética, sino a la resolución de problemas logísticos reales. Enfrentarnos a las debilidades de una página real nos ha obligado a pensar como arquitectos de información
y gestores de eventos simultáneamente.


>>>> Este fichero se debe editar para que cada evidencia quede enlazada con el recurso subido a la carpeta de la practica. Se pide más detalle técnico en las descripciones de lo que sería el README principal del repositorio y que corresponde a la descripcion del Case Study.
>>>> Termine con la seccion de Conclusiones para aportar una valoración final del equipo sobre la propia realización de la práctica
