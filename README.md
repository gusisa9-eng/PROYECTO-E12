# Nombre del proyecto

Equipo E12 · Análisis de Datos Básico · Estud-IA (Capa 2)

> **Cómo llenar este archivo:** borra «Escribe aquí» y responde debajo de cada pregunta. Si todavía no sabes algo, escribe **PENDIENTE:** y qué te falta confirmar. No inventes datos.

## Ficha del proyecto · versión 1

### 1. Usuario y decisión
> ¿Quién usará el resultado (una persona o un área) y qué va a decidir con él?

La usaría un empresario o un programa de apoyo a Mipymes que necesita decidir en qué sectores enfocarse. 

### 2. Pregunta principal
> Una sola pregunta que ayude a tomar esa decisión.

¿Qué tan competido está mi sector?

### 3. Fuente de datos
> Enlace o nombre de la fuente. ¿Es pública o es una muestra de práctica inventada (sintética)? Si es inventada, dilo aquí.

https://www.datos.gov.co/Comercio-Industria-y-Turismo/Estructuraempresarial-Medell-n-seg-n-comunas-y-di/2zc9-bpzw/data_preview de la camara de comercio de medellin, es publica


### 4. Qué representa una fila
> Completa la frase: «Cada fila es…». ¿Qué campo distingue una fila de otra?
Cada fila representa el conteo de empresas registradas en Medellín para un año específico y una rama de actividad económica (División CIIU), distribuidas por comunas y corregimientos, es un sector en un año; lo que diferencia exactamente una fila de otra es la combinación única de dos variables: el Año (AÑO) y el Grupo de Actividad Económica (División / Descripción)


### 5. Periodo
> ¿Qué fechas cubren los datos?

Del 2018 al 2022.

### 6. Cuatro indicadores
> Nombre de cada indicador y, si ya puedes, cómo se calcula (qué se divide entre qué).

1. Tasa de Crecimiento Neto Empresarial (2018 vs. 2022)
2. Índice de Concentración Territorial (Top 3 Comunas en 2022)
3. Participación por Sector Económico en 2022 (Vocación Productiva)
4. Dinamismo del Sector Cuaternario vs. Comercio Tradicional (2018–2022)

### 7. Fuera de alcance
> Lo que este proyecto NO va a responder.

No es posible conocer el número exacto de empresas creadas ni liquidadas por separado, pero sí puedes calcular la variación neta anual (el saldo de empresas que aumentaron o disminuyeron cada año) por cada sector económico.
## Si alcanzas hoy (para el jueves es obligatorio)

### Dos comparaciones útiles
> Por ejemplo: por mes, por comuna, por categoría.

1. Medellín vs. Resto de Antioquia (Descentralización y Oportunidad Regional)
2. Comunas Tradicionales vs. Comunas de Expansión (Saturación vs. Crecimiento 2018–2022)

### Tres riesgos de calidad
> ¿Qué podría venir mal en los datos? ¿Qué harías si la fuente falla?

1. Sesgo de "Domicilio Administrativo" vs. "Operación Real":
2. Rupturas metodológicas por depuración (Saltos artificiales)
3. Subregistro de informalidad: 
Si la fuente falla:
1. Aislar y auditar los datos sucios (Control de calidad en Excel)
2. Cruzar con fuentes oficiales alternativas (Triangulación), Rues, Dane, Alcaldia de medellin
### Mapa de preguntas
- ¿Qué pasó? Errores ocultos que suelen traer estas bases de datos empresariales (como direcciones administrativas en El Poblado o corregimientos en cero antes de 2021) 
- ¿Dónde o cuándo es distinto? Esos errores están en las dos bases de datos originales (los archivos CSV) que subi al inicio, específicamente en el sistema de registro de la fuente (Cámara de Comercio) antes de que los abriera en Excel.
- ¿Qué recomendaría y con qué límites? Resumiendo se recomienda usar las tablas como una guía de densidad competitiva y crecimiento relativo en 2022, filtrando previamente las categorías sin clasificar y cruzando los hallazgos con datos de ventas o empleo real.

## Archivos del proyecto

| Archivo o carpeta | Qué contiene |
|---|---|
| [diccionario.md](diccionario.md) | Qué significa cada columna de la muestra |
| [bitacora.md](bitacora.md) | Decisiones y por qué; uso de IA |
| `datos/originales/` | La muestra tal como se descargó (no se modifica) |
| `consultas/` | Consultas SQL comentadas (sesión 3) |
| `notebooks/` | Cuadernos de Colab (sesiones 3 a 5) |
| `tablero/` | Capturas y enlace del tablero (sesión 6) |

## Reglas del repositorio

- Es **público**: nada de datos personales (nombres, cédulas, teléfonos, correos, direcciones), contraseñas ni llaves.
- Lo que está en `datos/originales/` no se modifica: se guarda tal como se descargó.
- Cada commit dice en su mensaje **qué** se decidió y **por qué**.

---

Proyecto desarrollado en Estud-IA · Capa 2 · Análisis de Datos.
