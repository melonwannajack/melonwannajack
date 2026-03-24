# Análisis de Variable Real

## 1. Qué es
Formalización rigurosa del cálculo en ℝ. Estudia límites, continuidad, derivadas e integrales desde axiomas 
(completitud de ℝ), con foco en precisión lógica y control de errores.

## 2. Ideas clave

- Límite como noción central (ε-δ)
- Completitud de ℝ (supremo, ínfimo)
- Continuidad como estabilidad local
- Derivada como límite de variaciones
- Integral como acumulación (Riemann)

## 3. Intuición

Es pasar de “funciona en ejemplos” a “funciona siempre”.  
Todo se reduce a controlar cuánto se acerca algo a otra cosa.

La clave no es calcular, sino **acotar**.

## 4. Herramientas principales

- Definición ε-δ de límite
- Teorema del valor intermedio
- Teorema de Bolzano-Weierstrass
- Teorema de Heine-Borel
- Teorema fundamental del cálculo
- Criterios de convergencia de sucesiones y series

## 5. Ejemplos tipo
- Demostrar que una sucesión converge
- Ver si una serie converge o diverge
- Probar continuidad o no continuidad
- Estudiar extremos de funciones
- Justificar intercambios de límite/integral (casos básicos)

## 6. Conexiones
- → Probabilidad: base de medida e integración
- → Ecuaciones diferenciales: comportamiento de soluciones
- → Métodos numéricos: aproximaciones controladas
- → Análisis funcional: generalización a espacios abstractos

## 7. Lo que me costó
- Entender ε-δ sin verlo como formalismo vacío
- Interiorizar completitud (no es obvio por qué importa)
- Separar intuición gráfica de prueba rigurosa

## 8. Lo que me cambió la cabeza
Que casi todo se reduce a:
- elegir bien ε
- construir una cota

Y que ℝ no es “los números de siempre”, sino un objeto con propiedades muy específicas (completitud) que hacen que todo funcione.

## 9. Nivel actual
Parcial.  
Conceptos claros, pero falta agilidad en demostraciones formales.

## 10. Si tuviera que reaprenderlo
- Enfocar primero en:
  - sucesiones
  - completitud
- Luego continuidad → derivadas → integrales
- Priorizar demostraciones cortas y repetidas
- Implementar ejemplos en Python para reforzar intuición

## 11. Núcleo mínimo (lo imprescindible)
- Definición de límite (ε-δ)
- Supremos e ínfimos
- Continuidad
- Teorema fundamental del cálculo

## 12. Señales de dominio
- Poder demostrar convergencia sin mirar apuntes
- Entender cuándo una intuición falla
- Construir contraejemplos simples

## 13. Anti-patrones
- “Esto es obvio” sin justificar
- Confiar solo en gráficas
- Memorizar teoremas sin entender hipótesis

## 14. Ejemplo canónico

Probar que:

lim (n→∞) 1/n = 0

Idea:
Para cualquier ε > 0, elegir N > 1/ε  
Entonces si n > N → 1/n < ε

→ Control directo por desigualdad

## 15. Conexión personal
Fue el punto donde las matemáticas dejaron de ser cálculo y pasaron a ser estructura lógica.  
Marcó la diferencia entre “resolver ejercicios” y “entender por qué funciona”.
