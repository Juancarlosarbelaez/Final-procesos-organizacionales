# Eco-Moda S.A.S. - Transformación Digital

## Proyecto final de **Procesos Organizacionales** 
---

## 📋 Tabla de Contenidos

- [Descripción del Proyecto](#-descripción-del-proyecto)
- [Estructura del Repositorio](#-estructura-del-repositorio)
- [Componentes del Proyecto](#-componentes-del-proyecto)
- [Tecnologías Utilizadas](#-tecnologías-utilizadas)
- [Instalación y Ejecución](#-instalación-y-ejecución)
- [Fuentes de Datos](#-fuentes-de-datos)
- [Equipo de Trabajo](#-equipo-de-trabajo)
- [Información Académica](#-información-académica)

---

## 📋 Descripción del Proyecto

Desarrollo de una estrategia integral de datos para **Eco-Moda S.A.S.**, empresa de moda sostenible que enfrenta desafíos de competitividad digital. El proyecto abarca desde la formulación estratégica hasta la implementación técnica, incluyendo análisis de datos, modelado de procesos y gobierno de datos.

**Problema central**: Disminución de ventas por estructura organizacional rígida, presencia digital limitada y falta de integración entre canales físicos y digitales.

**Solución propuesta**: Transformación digital basada en datos, con automatización de procesos, integración omnicanal y marco de gobierno de datos.

---

## 📁 Estructura del Repositorio
```
Final-procesos-organizacionales/
│
├── 📊 dashboard/                          # Dashboard de visualización
│   └── dashboard_ECOMODA.pbit             # Dashboard de Power BI
│
├── 📦 data/                               # Datos procesados
│   └── datos_cleaned.csv                 # Dataset limpio y normalizado
│
├── 📚 documentacion/                      # Documentación completa del proyecto
│   ├── Definición del problema, necesidad del negocio y estrategia.pdf
│   ├── Diagrama_BPMN.pdf                 # Procesos modelados en BPMN
│   ├── Gobierno_Datos.pdf                # Roles, reglas y estándares
│   └── Pipeline_ArquitecturaDatosEcoModa.pdf #Borrador arquitectura de datos
│
├── 📓 notebooks/                          # Notebooks de análisis
│   ├── Limpieza_datos_completos.ipynb    # 1. Limpieza y normalización
│   └── EDA.ipynb                         # 2. Análisis exploratorio
│
├── 📄 README.md                           # Este archivo
└── 📋 requirements.txt                    # Dependencias Python
```
---

## 🎯 Componentes del Proyecto

### 1. **Estrategia Corporativa**
Análisis del problema de negocio y definición de estrategia de transformación digital basada en cuatro pilares: rediseño estructural, transformación digital, sostenibilidad e innovación, y crecimiento rentable.

📄 **Ver documento completo**: [`documentacion/Definición del problema, necesidad del negocio y estrategia.pdf`](documentation/Definición%20del%20problema,%20necesidad%20del%20negocio%20y%20estrategia.pdf)

---

### 2. **Modelado de Procesos (BPMN)**
Diagramas de procesos clave del negocio utilizando notación BPMN 2.0:
- Proceso de Ventas Omnicanal

📄 **Ver diagramas**: [`documentacion/Diagrama_BPMN.pdf`](documentacion/Diagrama_BPMN.pdf)

---

### 3. **Arquitectura de Datos**
Diseño técnico del pipeline de datos que incluye capas de ingesta, procesamiento, almacenamiento y consumo.

📄 **Ver arquitectura**: [`documentacion/Pipeline_ArquitecturaDatosEcoModa.pdf`](documentation/Pipeline_ArquitecturaDatosEcoModa.pdf)

---

### 4. **Gobierno de Datos**
Marco de gobierno que define:
- Roles y responsabilidades (CDO, Data Stewards, Data Engineers)
- Reglas de calidad (completitud, unicidad, rangos válidos)
- Estándares de nomenclatura y formato

📄 **Ver documento completo**: [`documentacion/Gobierno_Datos.pdf`](documentation/Gobierno_Datos.pdf)

---

### 5. **Análisis de Datos**
Procesamiento y análisis exploratorio implementado en notebooks Python:

#### Notebook 1: Limpieza de Datos
- Carga de datos crudos: consolidación dataset
- Aplicación de reglas de calidad
- Normalización y estandarización
  
- **Ejecutar**: `notebooks/Limpieza_datos_completos.ipynb`

#### Notebook 2: Análisis Exploratorio (EDA)
- Análisis descriptivo de ventas y clientes
  **Análisis realizados**:
- Estadísticas descriptivas y distribuciones
- Detección de valores nulos y outliers
- Análisis de correlaciones entre variables
- Segmentación de clientes y productos
- Identificación de patrones temporales
  
- **Ejecutar**: `notebooks/EDA_proyecto.ipynb`

---

### 6. **Dashboard de Visualización**
Dashboard interactivo desarrollado en **Microsoft Power BI** para la toma de decisiones estratégicas.
**Características implementadas**:
  1. Segmentación de clientes por estado de membresía (donut chart)
  2. Análisis de productos por categoría y color (barras horizontales)
  3. Preferencias por edad y color (líneas múltiples)
  4. Tendencias temporales 2018-2022 (serie de tiempo)

📊 **Ubicación**: `dashboard/dashboard_ECOMODA.pbit`  

---

## 🛠️ Tecnologías Utilizadas

- **Lenguajes y Frameworks**: Python 3.8+, PySpark
- **Análisis y Procesamiento de Datos**: Pandas, NumPy, PySpark SQL
- **Visualización**: Matplotlib, Seaborn, Microsoft Power BI
- **Herramientas de Desarrollo**: Jupyter Notebook, VS Code
- **Modelado de Procesos**: Bizagi Modeler (BPMN 2.0)
- **Control de Versiones**: Git & GitHub

---

## 🚀 Instalación y Ejecución

### Paso 1: Clonar el repositorio
```bash
git clone https://github.com/[TU-USUARIO]/Final-procesos-organizacionales.git
cd FINAL-PROCESOS-ORGANIZACIONALES
```

### Paso 2: Instalar dependencias
```bash
pip install -r requirements.txt
```

### Paso 3: Ejecutar notebooks
```bash
jupyter notebook
```

**Orden de ejecución recomendado**:
1. `Limpieza_datos_completos.ipynb`
2. `EDA_proyecto.ipynb`

**Nota**: El Notebook 1 requiere PySpark para procesar los 3.25GB de datos eficientemente.

### Paso 4: Visualizar el Dashboard
1. Instalar Power BI Desktop: https://powerbi.microsoft.com/desktop/
2. Abrir: `dashboard/dashboard_ECOMODA.pbix`
3. Actualizar conexión de datos si es necesario

---

## 📊 Fuentes de Datos

**Dataset principal**: https://www.kaggle.com/datasets/fashionworldda/fashion-trend-dataset?resource=download 
- **Descripción**: Dataset de productos de moda que captura tendencias, preferencias y métricas de ventas en el período 2018-2022. Contiene información detallada sobre productos de moda incluyendo preferencias de género, categorías, patrones, colores, grupos de edad objetivo, preferencias estacionales, materiales, precios, conteo de ventas, reseñas y calificaciones.
- **Período**: 2018 - 2022
- **Registros**: 31788324
- **Variables clave**: transaction_date, product_group_name, price, age, club_member_status

---


## 👥 Equipo de Trabajo

| Integrante           | GitHub                                   |                               
|----------------------|------------------------------------------|
| Juan Carlos Arbelaez | [@Juancarlosarbelaez](https://github.com/Juancarlosarbelaez) | 
| Manuela Gómez        | [@manugomez1206](https://github.com/manugomez1206) | 
| Alexandra Vasco      | [@botanicalex](https://github.com/botanicalex) | 

---

## 🎓 Información Académica

**Universidad**: Universidad Pontificia Bolivariana  
**Materia**: Procesos Organizacionales  
**Docente**: María Victoria Valencia Arango  
**Fecha de entrega**: Noviembre 24, 2024  

---
