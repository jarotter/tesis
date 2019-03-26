# Tesis

Recientemente, la atención popular en el aprendizaje de máquina se ha enfocado
en el *deep learning*, (redes neuronales profundas que se han probado
exitosas en reconocimiento de imágenes y análisis de texto) y en métodos
para grandes volúmenes de datos. Sin embargo, casi todos los algoritmos de
aprendizaje modernos utilizan técnicas de optimización  que dificultan
cuantificar la incertidumbre. Encontrar equivalentes bayesianos es difícil,
pues incluso los modelos más clásicos son difíciles de escalar a la complejidad
y el volumen de los datos que han dado éxito a su contraparte frecuentista. 
En este trabajo se explorará un algoritmo de inferencia variacional propuesto
por Liu y Wang (SVGD). Este algoritmo combina la flexibilidad no-paramétrica de 
los métodos MCMC con la facilidad de cómputo de los métodos variacionales.

SVGD plantea aproximar la posterior con partículas que se actualizan
iterativamente para reducir la divergencia de Kullback-Leibler desde la medida
empírica de las partículas hacia la posterior. Para facilitar el cómputo, elige 
como espacio para la optimización la bola unitaria de un 
*reproducing kernel hilbertspace (RKHS)* y utiliza un resultado que liga 
la derivada de la divergencia de Kullback-Leibler con la discrepancia de Stein, 
que surge en el método de Stein utilizado para acotar aproximaciones de momentos. 
Mostraremos que el algoritmo puede interpretarse como una forma de descenso en 
gradiente funcional en este RKHS y como un método para que la
esperanza de todas las funciones en cierto conjunto, relativo a la medida
empírica de las partículas, coincida con la de relativa a la posterior. Esta
última interpretación además pone en perspectiva el efecto que la elección del
kernel tiene sobre la convergencia del algoritmo.

