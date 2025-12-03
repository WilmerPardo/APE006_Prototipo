# Documentación de Flujo y Pantallas - Mi Diario Ganadero

## Descripción del Flujo
El flujo del proyecto "Mi Diario Ganadero" abarca la gestión integral del ciclo de vida del ganado en una finca. Comienza con una visión general del estado de la finca en el Dashboard, permitiendo navegar hacia la administración detallada del inventario activo y sus filtros. El sistema facilita la entrada de nuevos animales mediante formularios de registro y la consulta profunda de cada individuo a través de su ficha técnica y hoja de vida. Paralelamente, se gestionan procesos críticos como el control sanitario y tratamientos, así como el registro histórico de animales que han salido del inventario por venta o deceso. Finalmente, el flujo se cierra con herramientas de análisis de datos para la toma de decisiones y la personalización de la identidad de la finca.

---

## Detalle de Pantallas

### 1. Dashboard / Inicio
* **Nombre del archivo:** `index.html`
* **Propósito:** Proporcionar un resumen ejecutivo inmediato sobre el estado operativo y productivo de la finca.
* **Componentes Principales:**
    * **Barra lateral de navegación:** Menú persistente para acceso a módulos.
    * **Tarjetas de KPIs:** Indicadores numéricos de Total de Animales, Enfermos, Ventas y Nacimientos con tendencias porcentuales.
    * **Botones de Acción Rápida:** Acceso directo a "Añadir Nuevo Animal" y "Registrar Venta".
    * **Gráficos Resumen:** Visualización de la composición del rebaño (por categoría) y evolución del inventario.

### 2. Inventario General
* **Nombre del archivo:** `inventario.html`
* **Propósito:** Listar, buscar y filtrar la totalidad de los animales activos en la finca para su gestión rápida.
* **Componentes Principales:**
    * **Barra de Herramientas:** Buscador general y botón para registro de animales.
    * **Panel de Filtros:** Opciones laterales para filtrar por Raza, Sexo, Grupo de Edad y Estado.
    * **Tabla de Datos (Responsive):** Listado con Foto, ID/Arete, Nombre, Raza, Sexo, Edad y Estado.
    * **Menú de Acciones:** Botón de "más opciones" (...) por fila para editar o ver detalles.

### 3. Registro de Nuevo Animal
* **Nombre del archivo:** `nuevo_animal.html`
* **Propósito:** Capturar la información inicial para dar de alta a un nuevo integrante en el rebaño.
* **Componentes Principales:**
    * **Área de Carga de Imagen:** Zona para subir la fotografía del animal.
    * **Formulario de Datos Básicos:** Campos de texto para Código/ID y Nombre.
    * **Selectores:** Listas desplegables para Raza y botones de opción (radio buttons) para Sexo.
    * **Selector de Fecha:** Input para fecha de nacimiento.
    * **Botones de Control:** "Cancelar" y "Guardar Animal".

### 4. Detalle del Animal (Hoja de Vida)
* **Nombre del archivo:** `detalle_animal.html`
* **Propósito:** Mostrar la información completa, trazabilidad y cronología de eventos de un animal específico.
* **Componentes Principales:**
    * **Encabezado de Perfil:** Foto grande, ID, Nombre, Etiquetas de estado (Activo/En Tratamiento) y Botones de acción (Editar, Registrar Evento).
    * **Navegación por Pestañas:** Acceso a Datos Básicos, Historial Médico, Control de Peso y Eventos.
    * **Grid de Información:** Datos genealógicos (Padre/Madre), características físicas y ubicación actual.
    * **Línea de Tiempo:** Lista visual de eventos recientes (ej. Vacunación, Movimientos).

### 5. Gestión de Salud
* **Nombre del archivo:** `salud.html`
* **Propósito:** Monitorear y gestionar los animales que se encuentran enfermos o bajo tratamiento veterinario.
* **Componentes Principales:**
    * **Resumen Sanitario:** Contadores de animales en tratamiento y seguimientos pendientes.
    * **Herramientas de Gestión:** Buscador específico y botones de exportación/impresión.
    * **Tabla de Tratamientos:** Lista detallada con diagnóstico, fechas de inicio, fechas de próximo seguimiento (con alertas visuales) y estado de recuperación.

### 6. Historial de Eventos (Salidas)
* **Nombre del archivo:** `historial.html`
* **Propósito:** Consultar el registro de animales que ya no forman parte del inventario activo (ventas, muertes o pérdidas).
* **Componentes Principales:**
    * **Selector de Categoría:** Pestañas para alternar entre "Ventas" y "Pérdidas/Fallecimientos".
    * **Botón de Exportación:** Opción para descargar la data en CSV.
    * **Listado Histórico:** Tabla con foto, ID, Raza, Fecha de salida y Precio de venta (si aplica).

### 7. Reportes y Estadísticas
* **Nombre del archivo:** `reportes.html`
* **Propósito:** Visualizar métricas agregadas y gráficos para el análisis de rendimiento de la finca.
* **Componentes Principales:**
    * **Filtros Temporales:** Botones para seleccionar rangos de tiempo (ej. Últimos 30 días).
    * **Tarjetas Métricas:** Datos de Peso Promedio, Tasa de Mortalidad y Nuevos Nacimientos.
    * **Gráficos Detallados:** Barras de progreso para distribución por raza y gráfico de área para la tasa de mortalidad mensual.

### 8. Configuración
* **Nombre del archivo:** `configuracion.html`
* **Propósito:** Gestionar la información del perfil del usuario y los datos identitarios de la finca.
* **Componentes Principales:**
    * **Formulario de Usuario:** Campos para nombre de usuario y correo electrónico.
    * **Formulario de Finca:** Campos para nombre de la finca y ubicación geográfica.
    * **Gestión de Branding:** Área para visualizar, cambiar o quitar el logo de la finca.
    * **Acciones:** Botones para "Cancelar" o "Guardar Cambios".

---
**Recursos Visuales:** Las capturas de pantalla e imágenes de referencia correspondientes a cada pantalla se encuentran almacenadas en el directorio `docs/img/`.