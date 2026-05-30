## Practica 5: EVALUACION. Accesibilidad y pruebas de usabilidad A/B Testing

# Personas


| ID | Edad | Género | Nivel de competencia digital | Usa gafas/lentillas | Condiciones de iluminación | Dispositivo y resolución | Conocimiento previo sobre la app/estudio | ¿Ha participado antes en pruebas de usabilidad? | Rol |
|----|------|--------|------------------------------|---------------------|----------------------------|---------------------------|------------------------------------------|--------------------------------------------------|-----|
| 1  | 20   | Hombre | Avanzada                     |         lentillas   |                            |ordenador                  |maximo                                    |No                                                |desarrollador|
| 2  | 21   | Hombre | Avanzada                     |gafas                |                            |                           |maximo                                          | No                                                  |desarrollador     |
| 3  | 21   | Hombre | Avanzada                     |  gafas                   |                            |ordenador                           |nulo                                          |No                                                  |usuario final     |
| 4  | 20   | Hombre | Avanzada                     |No                     |                            |ordenador                           |medio                                          |No                                                  |usuario final     |
| 5  | 23   | Hombre  | Alta                        |No                     |                            |ordenador                           |nulo                                          |No                                                  |usuario final     |
| 6  | 45   | Mujer  | Baja                         |gafas                     |                            |ordenador                           |nulo                                          |No                                                  |usuario final     |
| 7  | 24   | Mujer  | Baja                         |No                     |                            |ordenador                           |nulo                                          |No                                                  |usuario final     |
| 8  | 50   | Hombre | Media                        |gafas                     |                            |ordenador                           |nulo                                          |No                                                  |usuario final     |
| 9  | 22   | Hombre | Avanzada                     |No                     |                            |ordenador                           |medio                                         |No                                                  |diseñador     |
| 10 | 22   | Hombre | Avanzada                     |No                     |                            |ordenador                           |medio                                          |No                                                  |diseñador     |

## Resultados Eye Tracking
- Persona id 1:
<img width="1920" height="3525" alt="image" src="https://github.com/user-attachments/assets/962ecf4e-6006-42b7-a395-29a980d07787" />
<img width="1920" height="1471" alt="image" src="https://github.com/user-attachments/assets/4643dcbe-a7a1-4b5c-8c33-0720a10a2dc3" />
<img width="1920" height="1893" alt="image" src="https://github.com/user-attachments/assets/b1a95d0e-c9a3-4d8d-8a1f-8d6ab71fff8c" />
<img width="1920" height="3332" alt="image" src="https://github.com/user-attachments/assets/43289540-7232-4767-8751-b6cb9e088ccb" />

  
- Persona id 2:
<img width="1920" height="3525" alt="image" src="https://github.com/user-attachments/assets/fc1c98c1-7d41-4c79-8534-2bdfde9cd44f" />
<img width="1920" height="1471" alt="image" src="https://github.com/user-attachments/assets/cbbba07d-9740-423f-ab67-b3b0b27e13d0" />
<img width="1920" height="1893" alt="image" src="https://github.com/user-attachments/assets/10ff8ab1-1f4a-4c5d-91b5-72f01779f7eb" />
<img width="1920" height="3332" alt="image" src="https://github.com/user-attachments/assets/a004498d-bfec-46de-8846-b7a757d18aec" />




  
- Persona id 9:
<img width="1920" height="3525" alt="image" src="https://github.com/user-attachments/assets/021db998-e558-4934-b368-af6c2364cb6f" />
<img width="1920" height="1471" alt="image" src="https://github.com/user-attachments/assets/dfec5a9d-c0a3-4aa9-b4ee-5185a877d32f" />
<img width="1920" height="1893" alt="image" src="https://github.com/user-attachments/assets/cfbcd6e3-8a4a-4d86-9dc3-5466793d7532" />
<img width="1920" height="3332" alt="image" src="https://github.com/user-attachments/assets/29d2923a-3d5f-4ea8-8d63-2ad9f0903d5c" />




# Tareas

1. Pedir un plato sin gluten
2. Hacer una reserva

## 📊 Resultados del Cuestionario SUS (Datos Cuantitativos)

Para medir la percepción subjetiva de usabilidad, se ha administrado el cuestionario estándar SUS (System Usability Scale) a una muestra de 10 usuarios. El estudio se ha planteado mediante un modelo A/B Testing (*Between-Subjects*), donde 5 usuarios evaluaron el Diseño A (nuestra propuesta) y 5 evaluaron el Diseño B (el prototipo asignado para auditoría).

Los datos han sido procesados mediante un análisis multivariable.

### 3.1. Puntuación Global (SUS Score)

<img width="765" height="783" alt="image" src="https://github.com/user-attachments/assets/ad9bffea-a08d-42f3-a180-c28c6dbc343d" />


La comparativa muestra una diferencia significativa en la percepción de los usuarios:
* **Diseño A:** Alcanza una puntuación media de **91.5/100**, lo que indica un sistema altamente intuitivo y libre de fricciones.
* **Diseño B:** Obtiene una puntuación de **60/100**, situándose por debajo de la media estándar de la industria (68). Esto denota que, aunque funcional, el sistema presenta barreras de usabilidad que deben ser corregidas.

### 3.2. Curva de Percentiles e Interpretación

<img width="761" height="776" alt="image" src="https://github.com/user-attachments/assets/888bbbd5-8274-4694-9c76-5d6d8340aea6" />


Al trasladar estos resultados a la curva de percentiles y la escala de grados (Adjetivos de Bangor):
* El Diseño A se sitúa en el percentil 99 (**Grado A - Best Imaginable**).
* El Diseño B se sitúa en el percentil 27 (**Grado D - Marginal / OK**). 
Además, destaca la alta **Desviación Estándar (25.12)** en el Diseño B, lo que indica que la experiencia fue muy irregular entre los distintos participantes (algunos lo encontraron aceptable, mientras que para otros resultó frustrante).

### 3.3. Análisis Detallado (Per Item Chart) centrado en Diseño B

<img width="764" height="802" alt="image" src="https://github.com/user-attachments/assets/96f0c241-108e-41c5-94fb-23b8d996d43e" />


Desglosando los resultados por pregunta para extraer áreas de mejora claras del Diseño B, destacamos los siguientes *insights*:

* **Baja intención de uso (Q1):** Es la métrica más penalizada. Los usuarios no sintieron deseo de utilizar el sistema de forma frecuente.
* **Inconsistencia Visual (Q6):** Los usuarios detectaron un nivel alto de inconsistencia en la interfaz, lo que probablemente generó confusión durante la navegación.
* **Punto fuerte (Q2):** Pese a los problemas de ejecución, la curva de complejidad innecesaria se mantuvo relativamente positiva. Esto sugiere que el modelo mental del usuario encaja con la idea base del equipo, pero falla en la disposición técnica de los elementos.

* # 5. Evaluación de Accesibilidad

## 5.1. Objetivo del análisis

El objetivo de esta evaluación es realizar un estudio de accesibilidad del **caso B**, teniendo en cuenta tanto el cumplimiento técnico del diseño como su relación con la normativa de accesibilidad web.

El análisis se basa en las **WCAG** (*Web Content Accessibility Guidelines*), que son las pautas de referencia para evaluar la accesibilidad de una interfaz web. Estas pautas se organizan en cuatro principios principales:

* **Perceptible**
* **Operable**
* **Comprensible**
* **Robusto**

Como nivel de conformidad se toma como referencia el nivel **AA**, que suele ser el estándar recomendado para sitios públicos, servicios digitales y páginas web profesionales. También se tiene en cuenta la norma **UNE-EN 301549**, relacionada con los requisitos de accesibilidad para productos y servicios TIC.

En este caso, al tratarse de un prototipo realizado en Figma, la evaluación debe entenderse como una **revisión preliminar de accesibilidad**. La comprobación definitiva debería realizarse cuando el diseño esté implementado como una página web real.

---

## 5.2. Herramientas de evaluación utilizadas

Para realizar el análisis de accesibilidad se han considerado herramientas automáticas habituales en este tipo de informes:

| Herramienta    | Uso principal                                                                                                                                           |
| -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Lighthouse** | Permite obtener una puntuación rápida de accesibilidad, rendimiento, buenas prácticas y SEO desde el navegador Google Chrome.                           |
| **WAVE**       | Permite detectar errores visuales de accesibilidad, problemas de contraste, falta de textos alternativos, estructura incorrecta y otros fallos comunes. |

Estas herramientas son útiles para detectar problemas técnicos, aunque no sustituyen por completo una revisión manual. Hay aspectos como la claridad del lenguaje, la facilidad de uso o la experiencia de navegación que también deben comprobarse de forma manual.

---

## 5.3. Resultados del análisis por categorías WCAG

---

# A. Perceptible

El principio **perceptible** indica que la información y los elementos de la interfaz deben poder ser percibidos correctamente por todos los usuarios, incluyendo personas con baja visión, daltonismo o dificultades visuales.

---

## Resultado 1: Posible falta de contraste en botones y textos secundarios

**Error detectado:**
En algunas zonas de la interfaz pueden aparecer textos sobre fondos claros, tarjetas visuales o botones con colores suaves. Esto puede provocar que el contraste entre el texto y el fondo no sea suficiente.

**Criterio WCAG incumplido:**
**1.4.3 - Contraste mínimo**

**Impacto:**
Los usuarios con baja visión, daltonismo o que utilicen pantallas con mala iluminación pueden tener dificultades para leer el contenido o identificar acciones importantes, como botones de reserva, selección o confirmación.

**Recomendación de mejora:**
Aumentar el contraste entre el texto y el fondo. Se recomienda usar colores más oscuros para el texto y comprobar el contraste con herramientas como WAVE o Lighthouse. Por ejemplo, evitar texto gris claro sobre fondo blanco y utilizar negro o tonos oscuros.

---

## Resultado 2: Imágenes e iconos sin alternativa textual definida

**Error detectado:**
En una interfaz con imágenes, iconos, mapas o botones visuales, es necesario que estos elementos tengan una descripción textual cuando aporten información importante. En el prototipo de Figma no se puede comprobar directamente si las imágenes tendrán atributo `alt` o si los iconos tendrán una etiqueta accesible.

**Criterio WCAG incumplido:**
**1.1.1 - Contenido no textual**

**Impacto:**
Los usuarios que utilizan lectores de pantalla podrían no comprender la función de una imagen, icono o botón si no existe un texto alternativo que explique su significado.

**Recomendación de mejora:**
Cuando se implemente el diseño en HTML, se deben añadir textos alternativos en imágenes informativas y etiquetas accesibles en botones con iconos.

Ejemplo:

```html
<img src="zona-reserva.jpg" alt="Imagen de una zona disponible para reserva">

<button aria-label="Abrir menú de navegación">
  ☰
</button>
```

Si la imagen es únicamente decorativa, debería marcarse como decorativa para que no interfiera con los lectores de pantalla.

---

# B. Operable

El principio **operable** indica que la interfaz debe poder utilizarse correctamente con diferentes métodos de entrada. No debe depender únicamente del ratón, sino que también debe ser accesible mediante teclado y tecnologías asistivas.

---

## Resultado 3: Navegación por teclado no garantizada

**Error detectado:**
El prototipo contiene varias zonas interactivas, como navegación, botones, filtros, tarjetas o elementos de selección. Es necesario comprobar que todos estos elementos puedan recorrerse usando la tecla `Tab` y activarse con teclado.

**Criterio WCAG incumplido:**
**2.1.1 - Teclado**
**2.4.7 - Foco visible**

**Impacto:**
Una persona que no pueda usar ratón podría tener dificultades para navegar por la página, seleccionar opciones o completar una reserva si los elementos interactivos no son accesibles mediante teclado.

**Recomendación de mejora:**
Todos los botones, enlaces, filtros y campos deben ser accesibles con teclado. Además, el foco debe ser claramente visible para que el usuario sepa en qué elemento se encuentra.

Ejemplo:

```css
button:focus,
a:focus,
input:focus,
select:focus {
  outline: 3px solid #005FCC;
  outline-offset: 3px;
}
```

---

## Resultado 4: Interacciones visuales que pueden depender demasiado del ratón

**Error detectado:**
Si la interfaz incluye un mapa, zonas seleccionables o tarjetas visuales, puede existir un problema si la interacción solo se puede realizar haciendo clic con el ratón.

**Criterio WCAG incumplido:**
**2.1.1 - Teclado**

**Impacto:**
Los usuarios que navegan con teclado, lectores de pantalla o dispositivos adaptados podrían no poder seleccionar una zona o completar una acción si no existe una alternativa accesible.

**Recomendación de mejora:**
Ofrecer una alternativa textual o mediante formulario para las zonas visuales. Por ejemplo, si existe un mapa interactivo, también debería existir un listado o desplegable con las mismas opciones.

Ejemplo:

```html
<label for="zona">Selecciona una zona disponible:</label>

<select id="zona" name="zona">
  <option value="zona-a">Zona A</option>
  <option value="zona-b">Zona B</option>
  <option value="zona-c">Zona C</option>
</select>
```

---

# C. Comprensible

El principio **comprensible** indica que la información debe presentarse de forma clara, coherente y fácil de entender. También afecta a formularios, mensajes de error, instrucciones y navegación.

---

## Resultado 5: Formularios o filtros con etiquetas poco claras

**Error detectado:**
En las zonas de reserva, selección o filtrado, los campos deben tener etiquetas claras. Si solo se usan placeholders o textos breves, el usuario puede no entender exactamente qué debe introducir o seleccionar.

**Criterio WCAG incumplido:**
**3.3.2 - Etiquetas o instrucciones**

**Impacto:**
Los usuarios con menos experiencia digital o con dificultades cognitivas pueden tener problemas para completar correctamente el formulario o entender qué información se solicita.

**Recomendación de mejora:**
Añadir etiquetas visibles y descriptivas a todos los campos. No se debería depender únicamente del placeholder como explicación.

Ejemplo:

```html
<label for="fecha">Fecha de la reserva</label>
<input id="fecha" type="date" name="fecha">

<label for="personas">Número de personas</label>
<input id="personas" type="number" name="personas" min="1">
```

---

## Resultado 6: Mensajes de error poco específicos

**Error detectado:**
Si el usuario no completa correctamente un formulario, el sistema debe mostrar un mensaje claro indicando qué campo está mal y cómo corregirlo. Un mensaje genérico como “Error” no sería suficiente.

**Criterio WCAG incumplido:**
**3.3.1 - Identificación de errores**

**Impacto:**
El usuario puede no saber qué debe corregir, lo que puede provocar frustración o abandono de la tarea.

**Recomendación de mejora:**
Mostrar mensajes de error concretos junto al campo correspondiente.

Ejemplo:

```html
<label for="fecha">Fecha de la reserva</label>
<input id="fecha" type="date" name="fecha" aria-describedby="error-fecha">

<p id="error-fecha">
  Debes seleccionar una fecha para continuar.
</p>
```

---

# D. Robusto

El principio **robusto** indica que el contenido debe estar correctamente construido para que pueda ser interpretado por navegadores, lectores de pantalla y otras tecnologías asistivas.

---

## Resultado 7: Necesidad de estructura HTML semántica

**Error detectado:**
Al convertir el prototipo de Figma en una página web real, existe el riesgo de construir la interfaz usando demasiados elementos genéricos como `div`, sin estructura semántica clara.

**Criterio WCAG incumplido:**
**4.1.2 - Nombre, función y valor**

**Impacto:**
Los lectores de pantalla podrían no interpretar correctamente la estructura de la página, los botones, los formularios o las secciones principales.

**Recomendación de mejora:**
Usar etiquetas HTML semánticas como `header`, `nav`, `main`, `section`, `footer`, `button`, `label`, `input` y `select`.

Ejemplo:

```html
<header>
  <nav>
    <a href="#inicio">Inicio</a>
    <a href="#reservas">Reservas</a>
    <a href="#contacto">Contacto</a>
  </nav>
</header>

<main>
  <section aria-labelledby="titulo-reserva">
    <h1 id="titulo-reserva">Reserva tu espacio</h1>
    <p>Selecciona una zona disponible y completa los datos de la reserva.</p>
  </section>
</main>
```

---

## Resultado 8: Idioma de la página no definido

**Error detectado:**
Cuando se implemente la página, debe indicarse correctamente el idioma principal del documento.

**Criterio WCAG incumplido:**
**3.1.1 - Idioma de la página**

**Impacto:**
Los lectores de pantalla pueden pronunciar incorrectamente el contenido si no saben que la página está en español.

**Recomendación de mejora:**
Definir el idioma principal en la etiqueta HTML.

Ejemplo:

```html
<html lang="es">
```

---

## 5.4. Resumen de errores detectados

| Categoría    | Error detectado                                                | Criterio WCAG                          | Impacto                                                                   | Recomendación                                  |
| ------------ | -------------------------------------------------------------- | -------------------------------------- | ------------------------------------------------------------------------- | ---------------------------------------------- |
| Perceptible  | Posible contraste insuficiente en botones o textos secundarios | 1.4.3 - Contraste mínimo               | Dificulta la lectura a usuarios con baja visión                           | Aumentar contraste entre texto y fondo         |
| Perceptible  | Imágenes o iconos sin alternativa textual                      | 1.1.1 - Contenido no textual           | Los lectores de pantalla no interpretan correctamente el contenido visual | Añadir `alt` o `aria-label`                    |
| Operable     | Navegación por teclado no garantizada                          | 2.1.1 - Teclado / 2.4.7 - Foco visible | Usuarios sin ratón pueden no completar acciones                           | Permitir navegación con `Tab` y foco visible   |
| Operable     | Interacciones visuales dependientes del ratón                  | 2.1.1 - Teclado                        | Dificulta el uso con teclado o tecnologías asistivas                      | Añadir alternativas como listas o desplegables |
| Comprensible | Formularios o filtros con etiquetas poco claras                | 3.3.2 - Etiquetas o instrucciones      | Puede generar confusión al usuario                                        | Añadir etiquetas visibles y claras             |
| Comprensible | Mensajes de error poco específicos                             | 3.3.1 - Identificación de errores      | El usuario no sabe cómo corregir el error                                 | Mostrar errores concretos junto al campo       |
| Robusto      | Falta de estructura HTML semántica                             | 4.1.2 - Nombre, función y valor        | Dificulta el uso con lectores de pantalla                                 | Usar etiquetas HTML semánticas                 |
| Robusto      | Idioma de la página no definido                                | 3.1.1 - Idioma de la página            | Lectura incorrecta por lectores de pantalla                               | Usar `<html lang="es">`                        |

---


