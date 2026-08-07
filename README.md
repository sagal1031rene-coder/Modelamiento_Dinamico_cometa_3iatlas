markdown
# Modelamiento Dinámico del Cometa
{!{Open en Colab}{https://google.com}{https://google.com}
{!{license: MIT}(https://shields.io)}(https.//opensource.org)
Este repositorio contiene el código fuente, los cuadernos de procesamiento y los datos complemenmtarios asociados al artículo de investigación en ciencias planetarias:
> **"Modelamiento Dinámico del cometa 3I/ATLAS"**
> *Autores: René Sagal.*
> Aceptado para publicación/Publicado en **Planetary and Space Science Elsevier)**, 2026.
> El objetivo principal de este proyecto es simular la evolución dinámica , calcular las fuerzas no gravitacionales y proyectar la trayectoria orbital del cometa interestelar 3I/ATLAS utilizando Python en entornos de nube (Google Colab).
# Estructura del Repositorio
*´/data´- Datos de efemérides del JPL, observaciones del MPC y vectores de estado.
*´/notebooks´- Cuadernos de Google Colab (´.ipynb´) con las simulaciones dinámicas.
*´/plots´- Gráficos de elementos orbitales y diagramas de dispersión generados para artículo.
## Requisitos y Dependencias
El código está optimizado para ejecutarse en **Google Colab**, lo que elimina la necesidad de configuraciones locales complejas. Las principales bibliotecas utilizadas son:
*´astropy´- - Gestión de unidades físicas, tiempos y transformaciones de coordenadas de referencia.
*´astroquery´- - Descarga automatizada de efemérides desde el sistema JPL HORIZONS.
*´rebound´o ´scipy´- Integración numérica de N-cuerpos para la evolución orbital.
*´matplotlib´ & ´seaborn´- - Generación de gráficos vectoriales de alta resolución aptos para Elsevier.
## Instrucciones de Uso (Reproducibilidad)
Para reproducir las simulaciones dinámicas y las figuras del artículo:
### Opción 1: Ejecutar en Google Colab (Recomendado)
1. Haz clic en el botón **Open in Colab** que se encuentra en la parte superior de este documento.
2. Inicia sesión en tu cuenta de Google.
3. Ejecuta de forma secuencial las celdas de código (Entorno de ejecución´ > ´Ejecutar todas´). El cuaderno se encargará de clonar automáticamente los datos necesarios.
### Opción 2: Configuración Local
Si prefieres utilizar tu propia máquina o servidor.
´´´bash
# 1. Clonar el repositorio
git clone https://github.com
cd Modelamiento_Dinamico_cometa_3iatlas
# Instalar dependencias
pip install -r requirements.txt
# Lanzar el entorno
jupyter notebook notebooks/modelamiento_3I_ATLAS.ipynb
## Origen de los Datos.
Los datos astrométricos y de órbita de base utilizados provienen de:
* **JPL Small-Body Database (SBDB)** y el sistema HORIZONS (NASA).
* + **Minor Plantet Center (MPC)** de la Unión Astronómica Internacional.
## Cómo Citar este Trabajo
Si utilizas total o parcialmente este código o los modelos dinámicos generados, por favor cita el artículo original de Elsevier:
´´´bibtex
@article{sagal2026atlas,
title={Modelamiento Dinámico del cometa 3I/ATLAS},
author={Sagal, René},
journal={Planetary and Space Science},
volume={XX},
pages={XXX---XXX},
year={2026},
publisher={Elsevier},
doi={INGRESA_EL_DOI_CUANDO_LO_TENGAS}
}
## Licencia
Este proyecto se distribuye bajo la Licencia MIT. Eres libre de adaptar, modificar y construir sobre este trabajo, siempre y cuando se otorguen los créditos correspondientes a la publicación académica original.
