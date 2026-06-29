# ♞ CHESSDX 360 - Diagnóstico Ajedrecístico Inteligente

![Badge](https://img.shields.io/badge/Versión-1.0-blue)
![Badge](https://img.shields.io/badge/Estado-Activo-green)
![Badge](https://img.shields.io/badge/Licencia-MIT-blue)
![Badge](https://img.shields.io/badge/HTML5-Puro-red)

---

## 📖 Descripción

**CHESSDX 360** es una plataforma web inteligente de **diagnóstico ajedrecístico** que funciona 100% localmente en tu navegador. Convierte posiciones, imágenes, FEN, PGN y prompts en diagnósticos completos con legalidad, severidad, mejor jugada, causas probables y recomendaciones.

**Sin servidores. Sin envío de datos. Completamente privado.**

---

## ✨ Características Principales

### 🎯 14 Módulos de Análisis
- 📷 **Captura por imagen** - Reconstrucción de posiciones desde fotos
- ✍️ **Entrada por prompt** - Análisis por texto natural
- ♟ **Tablero virtual** - Editor 8x8 interactivo
- 🏛 **Partidas famosas** - Identificación de cl��sicos históricos
- 💥 **Diagnóstico de derrota** - Análisis de errores en PGN
- 📰 **Problemas de periódico** - Resolución de mate/tácticas
- ⚔️ **Análisis táctico** - Detección de amenazas
- 🧠 **Análisis estratégico** - Planes posicionales
- ⚙️ **Motor de evaluación** - Cálculo de balance material
- 📚 **Base histórica** - Matching de partidas similares
- 🚪 **Aperturas** - Clasificación ECO
- ♔ **Finales** - Técnica de finales
- 📄 **Informes** - Generación PDF/HTML
- 🌐 **Redes virtuales** - Simulador social (no oficial)

### 💾 Funcionalidades
✅ Validación legal de posiciones  
✅ Cálculo de severidad (Verde/Amarillo/Naranja/Rojo)  
✅ Historial persistente en localStorage  
✅ Exportación de análisis a JSON  
✅ Modo claro/oscuro  
✅ Impresión y generación PDF  
✅ Responsive design (escritorio, tablet, móvil)  
✅ Sin dependencias externas  

---

## 🚀 Inicio Rápido

### 1. Descarga el archivo

**Opción A - Desde GitHub (recomendado):**
```bash
# Usa este enlace directo
https://raw.githubusercontent.com/JMiguelPed/AjedrezJM/main/Ajedrez%20Codigo.html
```

**Opción B - Clona el repositorio:**
```bash
git clone https://github.com/JMiguelPed/AjedrezJM.git
cd AjedrezJM
```

### 2. Abre en tu navegador

```bash
# Simplemente abre el archivo HTML
# Windows: Doble clic en "Ajedrez Codigo.html"
# Mac/Linux: Clic derecho → Abrir con → Chrome
```

### 3. ¡Listo! No requiere instalación

---

## 📋 Cómo Usar

### Escenario 1: Analizar una posición puntual
1. Selecciona módulo **"⚔️ Análisis táctico"**
2. Pega FEN o edita el tablero manualmente
3. Haz clic **"Generar diagnóstico"**
4. Verás riesgo (0-100), severidad y mejor jugada

### Escenario 2: Analizar una partida completa
1. Selecciona **"💥 Diagnóstico de derrota"**
2. Pega tu PGN en el campo correspondiente
3. Marca errores con `?` o `??` (opcional)
4. Genera diagnóstico → obtén causa de derrota

### Escenario 3: Resolver un problema
1. Selecciona **"📰 Problemas de periódico"**
2. Escribe en prompt: "Mate en 2" o "Gana pieza"
3. Carga la posición (FEN o imagen)
4. Verás la solución sugerida

### Escenario 4: Buscar partida famosa
1. Selecciona **"🏛 Partidas famosas"**
2. Escribe: "Fischer", "Capablanca", "Kasparov" o "Morphy"
3. Sistema busca en histórico
4. Propone partidas candidatas

---

## 🎨 Interfaz

```
┌─────────────────────────────────────────────────────┐
│  ♞ CHESSDX 360           [Diagnosticar][Demo][Modo] │
└─────────────────────────────────────────────────────┘

┌──────────────────┐  ┌─────────────────────────────┐
│   MÓDULOS (14)   │  │   MOTOR DIAGNÓSTICO         │
│ • 📷 Imagen      │  │ [Tablero 8x8 interactivo]   │
│ • ✍️ Prompt      │  │ Módulo, FEN, PGN, Imagen   │
│ • ♟ Tablero      │  │ [Generar diagnóstico]       │
│ • ...            │  │                              │
├──────────────────┤  ├─────────────────────────────┤
│   HISTORIAL      │  │   RESULTADO                 │
│ [Exportar]       │  │ ✅ Riesgo: 35/100           │
│ [Limpiar]        │  │ 🟡 Amarillo - Atención      │
│ • Diag 1         │  │ Problemas, Causas, Recs    │
└──────────────────┘  └─────────────────────────────┘
```

---

## 📊 Indicador de Severidad

| Color | Nombre | Significado |
|-------|--------|------------|
| 🟢 | Verde | Posición legal, sin problemas (75-95% confianza) |
| 🟡 | Amarillo | Atención requerida (50-74% confianza) |
| 🟠 | Naranja | Problema grave (25-49% confianza) |
| 🔴 | Rojo | Ilegal o error fundamental (0-24% confianza) |

---

## 💾 Almacenamiento Local

✅ **Historial automático** en `localStorage`  
✅ **Máximo 80 diagnósticos** guardados  
✅ **Persiste entre sesiones** (no se pierde al cerrar)  
✅ **Exportable a JSON** para backup  

```javascript
// Ubicación: localStorage["chessdx360_history_v1"]
// Contiene: Array de diagnósticos con timestamp, severidad, etc.
```

---

## 🛠️ Tecnología

- **HTML5** - Estructura semántica
- **CSS3** - Diseño responsivo y variables CSS
- **JavaScript Vanilla** - Sin frameworks, puro ES6+
- **LocalStorage API** - Persistencia de datos
- **FileReader API** - Carga de imágenes

**Tamaño total:** ~40 KB (todo en un archivo)

---

## 📚 Documentación Completa

Para guía detallada de uso, ve a:
📖 [GUIA_USO_CHESSDX360.md](./GUIA_USO_CHESSDX360.md)

Contiene:
- 14 módulos explicados
- Formatos soportados (FEN, PGN, Imagen)
- Interpretación de resultados
- FAQ y troubleshooting
- Tips y trucos

---

## ⚖️ Limitaciones (MVP)

⚠️ **Identificación histórica simulada** - No accede a base PGN real  
⚠️ **Motor simulado** - Usa heurística local, no Stockfish integrado  
⚠️ **Visión de imagen limitada** - Solo previsualización, sin OCR  
⚠️ **14 módulos básicos** - Versionable para expansión  

**Nota:** Diseñado para educación y análisis rápido, no para arbitraje oficial.

---

## 🔮 Roadmap (Versiones Futuras)

- [ ] Integración con Stockfish WASM
- [ ] OCR para reconocimiento de tableros
- [ ] Base PGN histórica completa (50M+ partidas)
- [ ] API REST para análisis remoto
- [ ] Exportación a múltiples formatos (PGN, PDF, SVG)
- [ ] Análisis de aperturas por ECO
- [ ] Modo multijugador online
- [ ] App móvil nativa

---

## 📝 Licencia

**MIT License** - Libre para usar, modificar y distribuir.

```
MIT License © 2024 JMiguelPed

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software to use, modify, and distribute.
```

---

## 🤝 Contribuciones

¿Quieres mejorar CHESSDX 360?

1. Fork el repositorio
2. Crea rama: `git checkout -b feature/tu-mejora`
3. Commit cambios: `git commit -m "Agrega feature X"`
4. Push: `git push origin feature/tu-mejora`
5. Abre Pull Request

---

## 📞 Soporte

| Problema | Solución |
|----------|----------|
| Tablero no aparece | Refresh navegador (F5) |
| FEN rechazado | Valida formato: 8 filas con `/` |
| Imagen no carga | Soporta JPG, PNG (máx 10MB) |
| Historial desaparece | Limpiaste caché; usa "Exportar" antes |
| PDF no genera | Prueba en Chrome con márgenes mínimos |

---

## 👤 Autor

**JMiguelPed** - Desarrollador ajedrecístico

- 🔗 GitHub: [@JMiguelPed](https://github.com/JMiguelPed)
- 📧 Email: jmpedrazaai1@gmail.com

---

## 🎓 Agradecimientos

Inspirado en:
- Leyes del Ajedrez FIDE
- Teoría de aperturas ECO
- Principios de finales técnicos
- Análisis táctico moderno

---

## 📊 Estadísticas

```
Versión:        1.0 (MVP)
Tamaño:         ~40 KB
Módulos:        14 funcionales
Formatos:       FEN, PGN, JPG, PNG
Navegadores:    Chrome, Firefox, Safari, Edge
Dispositivos:   PC, Tablet, Móvil
Base datos:     LocalStorage (80 históricos)
```

---

## 🚀 Próximos Pasos

1. **Descarga el archivo** desde `/Ajedrez Codigo.html`
2. **Abre en Chrome** (recomendado)
3. **Haz clic en "Demo"** para ver ejemplo
4. **Lee la guía** en [GUIA_USO_CHESSDX360.md](./GUIA_USO_CHESSDX360.md)
5. **Experimenta** con tus propias posiciones

---

**¡Diviértete analizando ajedrez! ♞**

---

<div align="center">

**⭐ Si te gusta, considera dar una estrella ⭐**

[Repositorio](https://github.com/JMiguelPed/AjedrezJM) • 
[Descargar](https://raw.githubusercontent.com/JMiguelPed/AjedrezJM/main/Ajedrez%20Codigo.html) • 
[Guía](./GUIA_USO_CHESSDX360.md)

</div>
