# mumuki-proyecto-base

El objetivo de este proyecto fue analizar el genoma de la bacteria Micromonospora sp.
Las especies de Micromonospora han sido reconocida durante mucho tiempo como una especie productora de gran cantidad de antibióticos.

Por lo que se tomó una secuencia de una especie de este género no identificada pero con una capacidad promisoria de síntesis de compuestos antimicrobianos comprobado mendiante la inhibición del crecimiento de cepas bacterianas tipo (ATCC).
A partir de la predicción de genes, se realizó una búsqueda de genes relacionados a la síntesis de antibióticos.

Este realiza la:
- Predicción de genes del genoma de Micromonospora sp. LH3U1
- Búsqueda de secuencias de proteínas de referencia relacionadas con la producción de antibióticos en la base de datos UniprotKB
- Análisis de homología con BLASTp
- Visualización de resultados de anotación con pyCirclize
- Análisis funcionales con InterPro

1. Paquetes requeridos para ejecutar el código:
  - pyCirclize: para visualizar nuestros datos genómicos
  - pyrodigal: para la predicción de genes codificantes
  - requests: para interactuar con las APIs de NCBI, UniProt e InterProScan
  - seaborn: para visualizar algunas de las propiedades genómicas obtenidas
  - subprocess: ejecutar comandos fuera del entorno de python
  - BioPython: para el manejo de secuencias
  - io: para conectar las entradas y salidas de los distintos programas
  - pandas:para el manejo general de datos

2. Programas adicionales

  - NCBI-Blast+: para comparar las secuencias

3. Corrida:

  Toda la información requerida para la ejecución del código se encuentra en el archivo Proyecto_final_WBDSLA.ipynb 
  Todo se ejecutó mediante el uso de Google Colaborative, por lo en el archivo encontrarán todos los códigos usado para el  análisis.

4. Archivos de entrada y salida

  *Archivos de salida*

- CP116936.1.blast.tsv
- CP116936.1.faa
- CP116936.1.gff

- candidates.gff
- uniprot_sequences.blast.tsv
- uniprot_sequences.fasta

5. Conclusiones

  Se logró extraer un operon relacionado a la producción de antibióticos en Micromonospora sp. y adicionalmente identificar las proteínas que conformaban este operon de manera funcional usando Interproscan.
  Sin embargo, cuando se realizó la búsqueda de operones encontramos muchos relacionados a producción de antibióticos, por lo cual sería necesario realizar un filtrado al momento de realizar la búsqueda de secuencias de referencias en Uniprot, de forma que tengamos un filtrado más específico de producción de antibióticos para este género.
