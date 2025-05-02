# Herramientas Open Source para Cómputo de Alto Desempeño (HPC)

El cómputo de alto desempeño (HPC) requiere herramientas eficientes para maximizar el uso de recursos como CPU, GPU y redes de interconexión en clústeres. A continuación se presenta una lista de herramientas **opensource** ampliamente usadas en entornos HPC, clasificadas por categoría:



##  Sistemas de gestión de recursos y colas de trabajo

### 1. SLURM (Simple Linux Utility for Resource Management)
- Gestor de colas más popular en sistemas HPC.
- Permite reservar nodos, ejecutar trabajos en lote o interactivos.
- Altamente escalable.
- [https://slurm.schedmd.com](https://slurm.schedmd.com)

### 2. PBS/Torque
- Evolución opensource de PBS (Portable Batch System).
- Menos usado que SLURM, pero aún presente en algunos centros de cómputo.

### 3. HTCondor
- Diseñado para trabajos de alto volumen y baja prioridad.
- Útil para cómputo distribuido sobre máquinas heterogéneas.



##  Librerías y entornos de programación paralela

### 1. MPI (Message Passing Interface)
- Estándar para programación paralela en clústeres.
- Implementaciones:
  - **OpenMPI**: [https://www.open-mpi.org](https://www.open-mpi.org)
  - **MPICH**: [https://www.mpich.org](https://www.mpich.org)

### 2. OpenMP
- Paralelismo a nivel de hilo para CPUs multinúcleo.
- Se usa con directivas en C, C++ y Fortran.

### 3. CUDA / ROCm
- **CUDA** (NVIDIA): no completamente open source.
- **ROCm** (AMD): sí es open source y creciente en soporte GPU.

### 4. Charm++
- Modelo de programación paralela orientado a objetos.
- Usado en simulaciones científicas (por ejemplo, NAMD).



## Bibliotecas científicas y numéricas

### 1. BLAS / LAPACK / ScaLAPACK
- Operaciones algebraicas optimizadas.
- Implementaciones: **OpenBLAS**, **ATLAS**, **Netlib LAPACK**.

### 2. PETSc
- Toolkit para ecuaciones diferenciales parciales en paralelo.
- [https://petsc.org](https://petsc.org)

### 3. Trilinos
- Módulos para álgebra lineal, solvers y optimización.
- [https://trilinos.github.io](https://trilinos.github.io)

### 4. FFTW (Fastest Fourier Transform in the West)
- Transformadas de Fourier en 1D, 2D y 3D.


## Contenedores y virtualización

### 1. Singularity
- Diseñado para HPC.
- Ejecuta contenedores sin necesidad de privilegios root.
- Compatible con Docker.

### 2. Apptainer
- Fork oficial de Singularity, mantenido por la Linux Foundation.
- [https://apptainer.org](https://apptainer.org)


## Monitoreo y gestión

### 1. Ganglia
- Sistema de monitoreo distribuido para clústeres.
- Visualización de CPU, RAM, red, etc.

### 2. Prometheus + Grafana
- Stack moderno para monitoreo.
- Visualización rica y personalizable.

## Otros frameworks y herramientas útiles

### 1. Hadoop / Spark (modo clúster)
- Más orientados a Big Data, pero útiles en tareas HPC.

### 2. Dask
- Computación paralela en Python.
- Escala desde laptops hasta clústeres.

### 3. JupyterHub
- Servidor multiusuario de notebooks Jupyter.
- Muy útil en entornos educativos y científicos.