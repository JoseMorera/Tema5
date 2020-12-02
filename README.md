---

## Universidad de Costa Rica
### Escuela de Ingeniería Eléctrica
#### IE0405 - Modelos Probabilísticos de Señales y Sistemas

Segundo semestre del 2020  
  
Laboratorio 5

---

* Estudiante: **José Alberto Morera Guzmán**
* Carné: **B85431**
* Grupo: **1**

---
Un servidor web es modelado como un sistema M/M/1 con una tasa de arribo de 2 solicitudes por minuto. La administración del servicio desea que el servidor no esté vacío (sin atender solicitudes) más del 10% del tiempo. Se debe hallar el parámetro 𝜈 para satisfacer este requisito y modificar el código para medir la variable de interés en una simulación. 
Para hallar el parámetro de servicio 𝜈 se lleva a cabo el despeje de la inecuación mostrada en el archivo L5.ipynb disponible en este repositorio. Se tiene que la probabilidad de que haya 1 o más personas en el sistema debe ser igual o mayor al 90% durate el día, con esto finalmente se llega a que 𝜈 debe ser igual o menor que 20/9, o bien 2.22 redondeado a dos decimales. 
