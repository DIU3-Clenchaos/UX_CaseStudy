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
