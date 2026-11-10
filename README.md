# Clases latentes bayesianas de los problemas por consumo de marihuana (ENCSPA 2019)

Cuaderno y datos del artículo *Análisis bayesiano de clases latentes de los
problemas asociados al consumo de marihuana en Colombia: asociaciones con
síntomas afectivos e inicio temprano de sustancias lícitas*
(Estadística Bayesiana & Pensamiento Crítico II, 2026-2,
Universidad Externado de Colombia).

Se identifican patrones latentes en 15 indicadores binarios de abuso y
dependencia (n = 1.217 consumidores recientes, 12 a 65 años) y se estima su
asociación con covariables sociodemográficas, síntomas de ánimo bajo e inicio
temprano de tabaco y alcohol. Clases y regresión se estiman de forma conjunta
(MCMC con NUTS, pseudo-verosimilitud ponderada por el factor de expansión).

## Cómo correrlo
1. `pip install -r requirements.txt` (Python 3.13).
2. Deja los csv de la ENCSPA 2019 en `ENCSPA_2019/`.
3. Abre `proyecto_bayesiana_encspa2019.ipynb` y ejecuta Kernel → Restart and run all.

Los resultados se guardan en `resultados/`. Los ajustes MCMC son lo más lento.
Las semillas están fijas, pero los valores exactos dependen de las versiones
de JAX y NumPyro.

## Datos
Microdatos anónimos de la ENCSPA 2019 (DANE). Los datos pertenecen al DANE y
se rigen por sus condiciones de uso.

## Autores
Juan Sebastian Sierra, Kenner David Lobo y Tomás Ávila.
