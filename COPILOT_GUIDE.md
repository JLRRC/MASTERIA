# Guía de Uso de GitHub Copilot en VSCode

Esta guía te ayudará a configurar y usar GitHub Copilot en Visual Studio Code para trabajar con el proyecto MASTERIA.

## Requisitos Previos

1. **Visual Studio Code** instalado ([Descargar aquí](https://code.visualstudio.com/))
2. **Cuenta de GitHub** con acceso a GitHub Copilot
3. **Suscripción a GitHub Copilot** ([Más información](https://github.com/features/copilot))

## Instalación de GitHub Copilot

### Paso 1: Instalar la Extensión de GitHub Copilot

1. Abre Visual Studio Code
2. Haz clic en el icono de Extensiones en la barra lateral izquierda (o presiona `Ctrl+Shift+X` / `Cmd+Shift+X`)
3. Busca "GitHub Copilot"
4. Haz clic en **Instalar** en la extensión oficial de GitHub Copilot
5. También instala **GitHub Copilot Chat** para obtener asistencia conversacional

### Paso 2: Iniciar Sesión en GitHub

1. Después de instalar la extensión, VSCode te pedirá que inicies sesión
2. Haz clic en **Sign in to GitHub**
3. Autoriza la extensión en tu navegador
4. Vuelve a VSCode una vez completado

### Paso 3: Verificar la Activación

1. Abre cualquier archivo de código (por ejemplo, un archivo `.py` o `.ipynb`)
2. Deberías ver el icono de Copilot en la barra de estado (esquina inferior derecha)
3. Si el icono tiene una marca de verificación, Copilot está activo ✓

## Uso de Copilot con Jupyter Notebooks

Este proyecto contiene Jupyter Notebooks para algoritmos y aprendizaje supervisado. Aquí te explicamos cómo usar Copilot con ellos:

### Configuración para Notebooks

1. Instala la extensión **Jupyter** en VSCode (si aún no la tienes)
2. Instala la extensión **Python** en VSCode
3. Copilot funcionará automáticamente en las celdas de código de los notebooks

### Trabajar con Notebooks

1. Abre un notebook (`.ipynb`) en VSCode
2. En una celda de código, comienza a escribir:
   - **Comentarios descriptivos**: Escribe `# Implementar algoritmo de optimización` y Copilot sugerirá código
   - **Código parcial**: Comienza a escribir una función y Copilot completará el resto
3. Acepta sugerencias con `Tab`
4. Navega entre sugerencias con `Alt+]` (siguiente) o `Alt+[` (anterior)

## Características Principales de Copilot

### 1. Autocompletado Inteligente

Copilot sugiere código mientras escribes. Simplemente comienza a escribir y:

- Presiona `Tab` para aceptar una sugerencia
- Presiona `Esc` para rechazarla
- Sigue escribiendo para ver nuevas sugerencias

### 2. Generación de Código desde Comentarios

Escribe comentarios descriptivos en español o inglés, y Copilot generará el código:

```python
# Crear una función para calcular la media de una lista
# Copilot generará la función completa
```

### 3. GitHub Copilot Chat

Usa Copilot Chat para obtener ayuda conversacional:

1. Abre el panel de Chat: presiona `Ctrl+Shift+I` / `Cmd+Shift+I`
2. Haz preguntas como:
   - "¿Cómo implemento un algoritmo genético en Python?"
   - "Explica este código"
   - "Optimiza esta función"
   - "Genera pruebas para este código"

### 4. Comandos Rápidos en Chat

- `/explain` - Explica el código seleccionado
- `/fix` - Sugiere correcciones para errores
- `/tests` - Genera pruebas unitarias
- `/doc` - Genera documentación

## Configuración Específica para MASTERIA

### Trabajar con Algoritmos de Optimización

Al trabajar en la carpeta `03MIAR Algoritmos de Optimización`:

1. Abre el archivo notebook
2. Escribe comentarios descriptivos sobre el algoritmo que necesitas
3. Ejemplo:
   ```python
   # Implementar algoritmo genético para el problema del viajante
   # con selección por torneo y crossover de un punto
   ```

### Trabajar con Aprendizaje Supervisado

Al trabajar en la carpeta `05MIAR_Aprendizaje_Supervisado`:

1. Copilot puede ayudarte con:
   - Preprocesamiento de datos
   - Implementación de modelos de ML
   - Visualización de resultados
   - Métricas de evaluación

2. Ejemplo:
   ```python
   # Crear un modelo de regresión logística con scikit-learn
   # incluyendo normalización de datos y validación cruzada
   ```

## Mejores Prácticas

### 1. Escribe Comentarios Claros

Los comentarios descriptivos ayudan a Copilot a generar mejor código:

```python
# ❌ Mal: # función
# ✓ Bien: # Función para calcular la distancia euclidiana entre dos puntos
```

### 2. Revisa las Sugerencias

Copilot es una herramienta de asistencia, no un reemplazo del pensamiento crítico:

- Revisa el código sugerido
- Verifica que sea correcto y eficiente
- Asegúrate de que siga las mejores prácticas

### 3. Usa Nombres Descriptivos

Variables y funciones con nombres claros ayudan a Copilot a entender el contexto:

```python
# ✓ Bien
def calcular_fitness_poblacion(poblacion, funcion_objetivo):
    pass

# ❌ Mal
def calc(p, f):
    pass
```

### 4. Proporciona Contexto

Incluye imports y definiciones relevantes en el mismo archivo para mejor contexto:

```python
import numpy as np
import pandas as pd
from sklearn.model_selection import train_test_split

# Ahora Copilot sabe que estás trabajando con estas bibliotecas
```

## Solución de Problemas

### Copilot no sugiere código

1. Verifica que el icono de Copilot esté activo en la barra de estado
2. Comprueba tu conexión a Internet
3. Reinicia VSCode
4. Verifica tu suscripción de Copilot en GitHub

### Sugerencias de baja calidad

1. Proporciona más contexto con comentarios
2. Usa nombres de variables más descriptivos
3. Incluye ejemplos o tipos en los comentarios
4. Asegúrate de tener los imports necesarios

### Copilot no funciona en Notebooks

1. Verifica que la extensión Jupyter esté instalada
2. Asegúrate de que el kernel de Python esté seleccionado
3. Recarga VSCode (`Ctrl+Shift+P` > "Reload Window")

## Atajos de Teclado Útiles

| Acción | Windows/Linux | macOS |
|--------|--------------|-------|
| Aceptar sugerencia | `Tab` | `Tab` |
| Rechazar sugerencia | `Esc` | `Esc` |
| Siguiente sugerencia | `Alt+]` | `Option+]` |
| Sugerencia anterior | `Alt+[` | `Option+[` |
| Abrir Copilot Chat | `Ctrl+Shift+I` | `Cmd+Shift+I` |
| Mostrar todas las sugerencias | `Ctrl+Enter` | `Ctrl+Enter` |

## Recursos Adicionales

- [Documentación oficial de GitHub Copilot](https://docs.github.com/en/copilot)
- [GitHub Copilot en VSCode](https://code.visualstudio.com/docs/editor/artificial-intelligence)
- [Mejores prácticas de Copilot](https://github.blog/2023-06-20-how-to-write-better-prompts-for-github-copilot/)

## Consejos Específicos para Este Proyecto

### Para Notebooks de Algoritmos

- Describe el problema en comentarios antes de escribir código
- Usa Copilot para generar funciones auxiliares
- Pide a Copilot que explique algoritmos complejos con `/explain` en Chat

### Para Aprendizaje Supervisado

- Copilot puede ayudar con pipelines de sklearn
- Usa comentarios para describir el preprocesamiento deseado
- Pide visualizaciones específicas (matplotlib, seaborn)

### Generación de Documentación

- Usa Copilot para generar docstrings
- Pide ejemplos de uso con `/doc` en Chat
- Genera explicaciones de código para tus compañeros

## Soporte

Si tienes problemas con Copilot:

1. Consulta la [documentación oficial](https://docs.github.com/en/copilot)
2. Revisa el [estado de GitHub](https://www.githubstatus.com/)
3. Contacta al soporte de GitHub si tienes problemas con tu suscripción

---

¡Esperamos que esta guía te ayude a aprovechar al máximo GitHub Copilot en tu trabajo con MASTERIA! 🚀
