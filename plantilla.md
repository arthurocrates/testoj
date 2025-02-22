# Impacto del Uso de Redes Sociales en la Salud Mental de Adolescentes  
**Autor**: Alex Johnson  
**Fecha**: 15 de octubre de 2023  
**Afiliación**: Universidad de Ciencias Digitales  

---

## Resumen  
Este estudio investiga la correlación entre el uso de redes sociales y la salud mental en adolescentes de 13 a 18 años. Se recopilaron datos mediante encuestas (*N* = 1.200) y se analizaron con modelos de regresión. Los resultados indican una asociación significativa entre la exposición prolongada a redes sociales y mayores niveles de ansiedad, aunque se requiere más investigación para establecer causalidad.  

**[Ir a Metodología](#metodología)** | **[Ir a Resultados](#resultados)**  

---

## Tabla de Contenidos  
1. [Introducción](#introducción)  
2. [Metodología](#metodología)  
3. [Resultados](#resultados)  
4. [Discusión](#discusión)  
5. [Conclusión](#conclusión)  
6. [Referencias](#referencias)  
7. [Apéndices](#apéndices)  

---

## Introducción <a name="introducción"></a>  
Las redes sociales se han integrado en la vida diaria de los adolescentes, con plataformas como TikTok e Instagram dominando sus rutinas. Si bien facilitan la conexión social, persisten preocupaciones sobre su impacto psicológico.  

### Preguntas de Investigación  
1. ¿Existe una correlación entre el uso diario de redes sociales y la ansiedad o depresión en adolescentes?  
2. ¿Algunas plataformas están más asociadas con efectos negativos en la salud mental?  

### Hipótesis  
- **H1**: Un mayor uso diario de redes sociales predice mayores niveles de ansiedad autoinformada.  
- **H2**: Plataformas centradas en imágenes (ej. Instagram) se correlacionan más con insatisfacción corporal.  

---

## Metodología <a name="metodología"></a>  
### Participantes  
- **Muestra**: 1.200 adolescentes (13–18 años) de escuelas urbanas y suburbanas.  
- **Distribución de género**: 58% mujeres, 40% hombres, 2% no binarios.  

### Instrumentos  
1. **Encuesta**: Cuestionario de 45 ítems sobre hábitos en redes sociales (ej. tiempo de uso, plataformas).  
2. **Métricas de Salud Mental**:  
   - Escala GAD-7 (Trastorno de Ansiedad Generalizada).  
   - Cuestionario PHQ-9 para depresión.  

### Procedimiento  
1. Los participantes completaron encuestas en línea de forma anónima.  
2. Los datos se analizaron con regresión lineal múltiple en R.  

```r
# Ejemplo de código en R para análisis de regresión
modelo <- lm(puntaje_ansiedad ~ tiempo_pantalla + genero + edad, data = datos_encuesta)
summary(modelo)
