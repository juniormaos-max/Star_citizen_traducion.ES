# 🚀 Star Citizen — Traducción al Español (ES / EN)

[![Versión](https://img.shields.io/badge/versión-4.10.2-blue.svg)](https://github.com/juniormaos-max/Star_citizen_traducion.ES/releases)
[![LIVE y PTU](https://img.shields.io/badge/compatible-LIVE%20%7C%20PTU-green.svg)](https://robertsspaceindustries.com)
[![Español España](https://img.shields.io/badge/variante-ES-red.svg)](https://github.com/juniormaos-max/Star_citizen_traducion.ES/releases)
[![Inglés Mejorado](https://img.shields.io/badge/idioma-EN-yellow.svg)](https://github.com/juniormaos-max/Star_citizen_traducion.ES/releases)

---

## 🎮 Sobre este proyecto

Traducción comunitaria del archivo de localización `global.ini` de **Star Citizen** al español, con soporte también para una versión en inglés mejorada.

- **ES** — español de España (vocabulario de España, uso de *vosotros*)
- **EN** — versión en inglés con todas las mejoras aplicadas (sufijos RS, firmas de escaneo, estadísticas, materiales, blueprints, mejoras de datos de crafting y minería)

El proyecto se construye sobre un pipeline propio de varias etapas de revisión y genera paquetes ZIP listos para instalar directamente en el juego.

> **Compatibilidad:** LIVE de Star Citizen.

---

## 🔀 ¿Qué versión elegir?

| Variante | Idioma | Región | Ideal para |
|----------|--------|--------|------------|
| **ES** | Español | España | Jugadores que prefieren el juego completamente en español |
| **EN** | Inglés | Internacional | Jugadores que quieren el juego en inglés con mejoras técnicas (RS, stats, blueprints, materiales) |

---

## 📥 Instalación paso a paso

1. **Descarga** la última versión desde los [releases](https://github.com/juniormaos-max/Star_citizen_traducion.ES/releases).
2. **Descomprime** el contenido del ZIP en la raíz de instalación de Star Citizen, por ejemplo:

   ```
   C:\Program Files\Roberts Space Industries\StarCitizen\
   ```

   El ZIP contiene la carpeta `LIVE/` con:
   - `LIVE/user.cfg` — configuración de idioma (`g_language = spanish_(spain)` o `g_language = english`)
   - `LIVE/data/Localization/spanish_(spain)/global.ini` — archivo de localización en español
   - `LIVE/data/Localization/english/global.ini` — archivo de localización en inglés mejorado

3. **Inicia el juego** y verifica que los textos aparezcan en el idioma seleccionado.

---

## ✅ ¿Qué está traducido / mejorado?

### Versión ES (Español de España)

| Sistema | Estado | Notas |
|---------|--------|-------|
| Interfaz de usuario (UI) | ✅ Traducido | Menús, HUD, pantallas, etiquetas |
| Misiones y contratos | ✅ Traducido | Títulos, detalles, reputación, recompensas |
| Minería y commodities | ✅ Traducido | Firmas de escaneo, ubicaciones, materiales |
| Crafting y fabricación | ✅ Traducido | Recetas, componentes, materiales |
| Ítems y equipamiento | ✅ Traducido | Armas, armaduras, escudos, motores |
| Pinturas de naves (Paint_*) | ✅ Traducido | Todas las claves de pintura traducidas |
| RS (firmas de escaneo de minería) | ✅ Añadido | Sufijo `(RS ####)` en los 26 tipos de mineral minable |
| Planetología Stanton | ✅ Traducido | Todos los planetas, estaciones, ubicaciones y descs |
| Pantalla de energía de nave | ✅ Traducido | `hud_Label_Offline`, `engineering_ui_Item_Output`, etc. |

### Versión EN (Inglés Mejorado)

| Sistema | Estado | Notas |
|---------|--------|-------|
| Interfaz de usuario (UI) | ✅ Inglés original | Todos los textos en inglés |
| Sufijos RS (minería) | ✅ Añadido | `(RS ####)` en los 26 tipos de mineral minable |
| Firmas de escaneo / datos de minería | ✅ Fusionados | Desde enhancement INIs (DataForge XML) |
| Estadísticas de ítems y componentes | ✅ Fusionadas | `components_desc_enhancements.ini`, `ships_desc_enhancements.ini`, `ship_weapons_desc_enhancements.ini`, `fps_weapons_desc_enhancements.ini`, `missile_enhancements.ini` |
| Blueprints y materiales de crafting | ✅ Fusionados | `commodity_crafting_enhancements.ini` |
| Consumibles médicos | ✅ Fusionados | `medical_consumables_enhancements.ini` |
| Diario | ✅ Fusionado | `journal_enhancements.ini` |
| Recompensas de misión | ✅ Fusionadas | `mission_rewards_enhancements.ini` |

---

## 🛠 Mejoras técnicas aplicadas

### RS (Resource Signature) en minería
Se añadió el sufijo `(RS ####)` a las 26 claves `mineabletype_primary_*` (agricium, aluminium, aslarite, beryl, bexalite, borase, copper, corundum, gold, hephaestanite, ice, iron, laranite, lindinium, ouratite, quantainium, quartz, riccite, savrillium, silicon, stileron, taranite, tin, titanium, torite, tungsten). Esto permite que las misiones de minería muestren la firma de escaneo de cada mineral en el diario del mobiGlas, en todas las ubicaciones (no solo en Battaglia). FOTOS MAS ABAJO CON LA INFORMACION.

### Pantalla de energía de nave
Se añadió `hud_Label_Offline` y se corrigió `engineering_ui_Item_Output` para que aparezcan correctamente en la interfaz de gestión de energía de la nave.

### Fusionado de enhancement INIs (versión EN)
Se fusionaron 9 archivos de enhancement generados desde DataForge XML (extraídos de Data.p4k con unp4k):
- `commodity_crafting_enhancements.ini` — materiales y datos de crafting
- `components_desc_enhancements.ini` — estadísticas de componentes de nave
- `ships_desc_enhancements.ini` — descripciones de naves
- `ship_weapons_desc_enhancements.ini` — armas de nave
- `fps_weapons_desc_enhancements.ini` — armas FPS
- `missile_enhancements.ini` — misiles
- `medical_consumables_enhancements.ini` — consumibles médicos
- `journal_enhancements.ini` — diario
- `mission_rewards_enhancements.ini` — recompensas de misión y blueprints

Total: **4,228 claves actualizadas** en la versión ES y en la EN con datos de blueprints, stats y materiales.

---

## 🤝 Soporte y comunidad

Si vas a crear una cuenta nueva en Star Citizen, se agradece si usas mi código de referencia:

**STAR-6W9K-GDJB**

👉 https://www.robertsspaceindustries.com/enlist?referral=STAR-6W9K-GDJB

Únete al Discord de la comunidad CCBE:

👉 https://discord.gg/8ZpvNM5qRB

Web de la compañía CCBE:

👉 https://ccbe.space/

---

## 🐛 Reportar errores o sugerencias

Si encuentras textos sin traducir, errores de ortografía o problemas con la instalación, abre un issue en el repositorio:

👉 [Nuevo issue en GitHub](https://github.com/juniormaos-max/Star_citizen_traducion.ES/issues)

👉 También puedes encontrarme en el Discord de la CCBE https://discord.gg/8ZpvNM5qRB para informar de errores de ortografía o problemas con la instalación.

Incluye:
- Versión del juego (LIVE)
- Variante instalada (ES / EN)
- Captura de pantalla del error (si aplica)
- Texto original y texto esperado

---

## 🏆 Créditos

- **Pipeline de traducción:** desarrollo propio con etapas de revisión (`rev1 → rev2 → rev3`)
- **Datos técnicos:** extraídos de los archivos DataForge de Star Citizen (crafting, minería, commodities)
- **Herramientas:** `unp4k` para extracción de Data.p4k, `generate_enhancements_ini.py` y `gen_commodity_crafting.py` y `global.ini` para generación de enhancement INIs
- **Imágenes y capturas:** aportes de la comunidad
- **Soporte:** comunidad CCBE y Discord

---

## 🖼️ Galería: antes y después

A continuación se muestran ejemplos reales de la traducción en el juego.

### Interfaz y estadísticas

![Estadísticas en español](imagenes/Screenshot_16.png)

Las estadísticas de armas y equipamiento (peso, cadencia, daño, DPS, munición, velocidad, alcance, consumo) aparecen con sus etiquetas en español.

### Materiales y fabricación

![Materiales de fabricación](imagenes/Screenshot_20.png)

Los materiales necesarios para fabricar cada objeto se muestran traducidos.

![Detalles y materiales de arma](imagenes/armakarna.png)

Detalles del arma y sus materiales, traducidos al español.

![Cargador](imagenes/cargador.png)

Ejemplo de componente con descripción en español.

### Minería y firmas de escaneo

![Firmas de escaneo](imagenes/Screenshot_25.png)

Tabla de firmas de escaneo en el diario de minería del mobiGlas: relaciona cada mineral con su firma para identificarlo al escanear.

![Ubicaciones de materiales](imagenes/hielopresu.png)

Las fichas de materiales incluyen sus ubicaciones (dónde encontrarlos) y los datos blueprint (en qué se usan para fabricar).

![Minería en misiones](imagenes/mineria.png)
![Minería en misiones](imagenes/mineria1.png)
![Minería en misiones](imagenes/mineria2.png)
![Minería en misiones](imagenes/mineria3.png)

En las misiones de minería o en las misiones de battaglia, los detalles de misión muestran las firmas de los materiales minables.

![Minería en misiones](imagenes/newbabbage.png)

### Antes y después: ascensor de Levski (Nyx)

![Antes: A ADUANAS](imagenes/levskiantes.png)

![Después: ADUANAS](imagenes/levskiahora.png)

Pantalla del ascensor en Nyx (Levski): antes ponía **CUSTOMS** y ahora **ADUANAS**.

![Aduana al salir del ascensor](imagenes/aduanaslesvki.png)

Al salir del ascensor en Levski está la aduana en el juego; en el `global.ini` se dejó tal cual: **ADUANAS**.

### Criaturas de New Babbage

![Cuasi pastador de la tundra](imagenes/cuasi.png)

Criaturas en New Babbage: **CUASI PASTADOR DE LA TUNDRA**.

### Contratos: antes y después

![Contratos antes](imagenes/contratos_antes.png)

![Contratos ahora](imagenes/contratos_ahora.png)

En los contratos, la reputación (rep) aparece en los detalles de cada misión, no solo en los títulos.

---

*Última actualización: versión compatible con Star Citizen 4.10.2*

