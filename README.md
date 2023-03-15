# Thermal Rectification

Repositorio de notebooks de Jupyter dedicados principalmente al cálculo de la Rectificación Térmica y la Difusividad Espectral presentes en el modelo de Fourier de una dimensión para una aleación de Silicio y Germanio. Dentro de los notebooks se explica con más detalle su descripción

## Para empezar

Es recomendable, además de contar con el software necesario, conocimiento sobre transferencia de calor y simulación numérica (diferencias finitas y Runge-Kutta de cuarto orden).

### Prerequisitos de software

* Alguna distribución reciente de Python
* Numpy, Scipy, Numba, matplotlib, Seaborn
* Jupyterlab o VSCode
* Opcionalmente, scienceplots. Nota: si no se desea emplear scienceplots hay que modificar o eliminar el estilo de graficación dentro de los notebooks.
* Es recomendable 

## Uso

Basta correr cada notebook en el orden que viene numerado.

* El solver se encuentra contenido en modulo_fourier.py, incluye funciones para calcular derivadas.
* Los notebook (a) se enfocan en el caso para obtener gráficas de linea. Los notebook (b) por su parte, son el caso para obtener gráficas heatmap.
* El notebook #0 es el generador de frecuencias para la posterior determinación las fronteras oscilantes.
* Los notebook #1 realizan el barrido de experimentos sobre el modelo de Fourier, es importante considerar que para tiempos de simulación largos y una gran cantidad de frecuencias, el total de simulaciones pueden tomar días de tiempo de ejecución.  
* Los notebook #2 generan las gráficas para la densidad espectral.
* Los notebook #3 generan las gráficas para la rectificación térmica empleando los datos obtenidos en los notebook #1.
* El notebook #4 realiza el cálculo y genera la gráfica de la velocidad de fase y la longitud de atenuación.
* El notebook #5 es el ejercicio de validación. Puede modificarse facilmente para realizar pruebas rápidas con el código.