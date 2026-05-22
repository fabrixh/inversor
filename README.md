# 📊 Radar del Inversor — Argentina

Dashboard gratuito de indicadores macroeconómicos de Argentina, diseñado como herramienta educativa para el curso **De Ahorrista a Inversor — Nivel II**.

Datos en tiempo real sin registro ni API key, usando únicamente APIs públicas y abiertas.

---

## 📈 Indicadores que muestra

| Indicador | Fuente | Actualización |
|---|---|---|
| 💵 Dólar MEP (bolsa) | dolarapi.com | Tiempo real |
| 💵 Dólar Blue | dolarapi.com | Tiempo real |
| 🔥 Inflación mensual (IPC) | argentinadatos.com / INDEC | Mensual |
| 🌡️ Riesgo País (EMBI) | argentinadatos.com / JP Morgan | Diaria |
| 🏦 Tasa Plazo Fijo TNA | argentinadatos.com / BCRA | Diaria |
| 🏛️ Reservas BCRA | api.bcra.gob.ar | Diaria |

Cada card incluye un **panel de fuentes** con links directos a INDEC, BCRA, Ámbito, Rava y más — para que el alumno pueda ir a la fuente original sin depender solo del dashboard.

---

## 🛠️ Instalación en GitHub Pages (paso a paso)

### Paso 1 — Crear el repositorio

1. Ingresá a [github.com](https://github.com) con tu cuenta
2. Hacé clic en **New repository**
3. Nombre sugerido: `radar-inversor-argentina`
4. Dejalo en **Public**
5. Hacé clic en **Create repository**

### Paso 2 — Subir el archivo

1. En tu repositorio vacío, hacé clic en **Add file → Upload files**
2. Subí el archivo `index.html` (renombrá `radar-inversor-argentina.html` a `index.html` antes de subirlo)
3. En el mensaje de commit escribí algo como: `primera versión del dashboard`
4. Hacé clic en **Commit changes**

### Paso 3 — Activar GitHub Pages

1. Andá a **Settings** (pestaña superior del repo)
2. En el menú izquierdo, hacé clic en **Pages**
3. En **Source**, seleccioná **Deploy from a branch**
4. En **Branch**, elegí `main` y la carpeta `/ (root)`
5. Hacé clic en **Save**

En 1-2 minutos tu sitio estará disponible en:
```
https://TU_USUARIO.github.io/radar-inversor-argentina/
```

---

## ⚠️ Nota técnica (CORS)

Las APIs usan restricciones CORS, por lo que el dashboard **no funciona abriéndolo como archivo local** (doble clic). Necesita correr desde un servidor web — GitHub Pages lo resuelve automáticamente.

Si querés probarlo en local antes de subir, podés usar:
```bash
# Con Python (si lo tenés instalado)
python3 -m http.server 8080
# Luego abrí: http://localhost:8080
```

---

## 🔗 APIs utilizadas

Todas gratuitas, abiertas y sin necesidad de registro:

- **[DolarApi.com](https://dolarapi.com)** — Cotizaciones del dólar en tiempo real (MEP, Blue, Oficial, CCL). Proyecto open-source.
- **[ArgentinaDatos.com](https://argentinadatos.com)** — Inflación, riesgo país, tasas, series históricas. Datos de BCRA e INDEC.
- **[API BCRA](https://www.bcra.gob.ar/apis-banco-central/)** — API oficial del Banco Central. Reservas, variables monetarias y cambiarias.

---

## 📚 Fuentes de información adicionales

Para cada indicador el dashboard incluye links a las fuentes primarias:

- [INDEC](https://www.indec.gob.ar) — IPC, EMAE, empleo, PBI
- [BCRA](https://www.bcra.gob.ar) — Tasas, reservas, política monetaria
- [Ámbito Financiero](https://www.ambito.com) — Mercados y tipo de cambio
- [InflacionReal.ar](https://www.inflacionreal.ar) — Mediciones privadas de inflación
- [Rava Bursátil](https://www.rava.com) — Mercado de capitales y dólar MEP
- [Dolarito.ar](https://dolarito.ar) — Comparador de tipos de cambio

---

## 🎓 Contexto educativo

Esta herramienta acompaña el módulo de **indicadores macroeconómicos** del curso *De Ahorrista a Inversor — Nivel II*, basado en el principio de que:

> *"Un inversor informado sigue datos de la economía real y del mercado para decidir mejor."*

El objetivo no es reemplazar el análisis propio, sino tener en un solo lugar los datos clave y saber dónde buscarlos cuando se necesite profundizar.

---

## 📄 Licencia

Uso educativo libre. Podés modificarlo y adaptarlo para tus clases.
