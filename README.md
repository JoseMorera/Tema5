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
Entre las modificaciones realizadas al código está la medición del tiempo cuando **no** hay ningún cliente en el sistema, este dato nos brinda información para obtener el porcentaje de tiempo total en el que el servidor está vacío, el cual no debería superar el 10% del tiempo total. Se tiene que si este porcentaje es menor a 10% se muestra el mensaje "Sí cumple con la especificación." y en caso que de tenga un porcentaje superior a 10% muestre el mensaje "No cumple con la especificación."  
Para interpretar la gráfica obtenida, se tiene que la línea roja es el umbral en el que hay una persona en el sistema, todos los datos por encima de esta línea es el tiempo en el que hay al menos una persona en el sistema (debe ser al menos el 90% del tiempo) y los que estén por debajo de está línea son los instantes en los que no hay al menos una persona en el sistema (debe ser igual o menor al 10% del tiempo total).  
En el resultado de una simulación se obtuvo:  
![Imgur](https://i.imgur.com/ZfIAWqX.png)  
Lo que quiere decir que el 9.78% del tiempo se tuvo 0 clientes en el sistema y corresponde a los momentos en la gráfica con datos por debajo de la línea roja.



