# 🚀 Star Citizen — Traducción al Español (ES / EN)

[![Versión](https://img.shields.io/badge/versión-4.10.3-blue.svg)](https://github.com/juniormaos-max/Star_citizen_traducion.ES/releases)
[![Compatible con LIVE](https://img.shields.io/badge/compatible-LIVE-green.svg)](https://robertsspaceindustries.com)
[![Español España](https://img.shields.io/badge/variante-ES-red.svg)](https://github.com/juniormaos-max/Star_citizen_traducion.ES/releases)
[![Inglés Mejorado](https://img.shields.io/badge/idioma-EN-yellow.svg)](https://github.com/juniormaos-max/Star_citizen_traducion.ES/releases)

---

> 🚀 **Última versión: 4.10.3-REV 3** . Incluye capturas nuevas y la corrección del problema que impedía mostrar la reputación (REP) y los planos en algunas misiones.

### Navegación

[Proyecto](#proyecto) · [Versiones](#versiones) · [Novedades](#novedades) · [Instalación y Descarga](#instalacion) · [Contenido](#contenido) · [Mejoras técnicas](#mejoras-tecnicas) · [Galería](#galeria) · [Comunidad](#comunidad) · [Errores](#errores) · [Créditos](#creditos)

<a id="proyecto"></a>
## 🎮 Sobre este proyecto

Proyecto comunitario de localización de **Star Citizen**, basado en el archivo `global.ini`. Incluye una versión en español de España y otra en inglés con mejoras de datos técnicos.

- **ES** — español de España (vocabulario de España, uso de *vosotros*)
- **EN** — inglés con mejoras de minería, firmas RS, estadísticas, materiales y planos de fabricación.

El proyecto utiliza un proceso propio de revisión y genera paquetes ZIP listos para instalar.

> **Compatibilidad:** Star Citizen LIVE.

---

<a id="versiones"></a>
## 🔀 ¿Qué versión elegir?

| Variante | Idioma | Región | Ideal para |
|----------|--------|--------|------------|
| **ES** | Español | España | Jugadores que prefieren el juego completamente en español |
| **EN** | Inglés | Internacional | Jugadores que quieren el juego en inglés con mejoras técnicas (RS, estadísticas, planos y materiales) |

---

<a id="novedades"></a>
## 🆕 Novedades — 4.10.3-REV 3

Esta revisión incluye imágenes nuevas y corrige un problema que impedía mostrar la reputación (REP) y los planos en algunas misiones.

<p align="center">
  <img src="imagenes/minerianaveantes.png" alt="Contratos de minería antes de los cambios" width="32%">
  <img src="imagenes/minerianaveahora.png" alt="Contratos de minería después de los cambios" width="32%">
  <img src="imagenes/nofallo.png" alt="Ejemplo de objetivo de minería generado dinámicamente" width="32%">
</p>

### Por qué el objetivo de minería aparece así

El objetivo de la captura —por ejemplo, «Entrega 0/4 SCU de Aluminio (RS 4285, 8570, 12855, 17140, 21425, 25710) a Complejo de producción Greycat Stanton IV-A en microTech»— no está guardado como una frase completa en `global.ini`. El juego la construye en tiempo real combinando la acción, el progreso, la cantidad, el material y el destino de la misión.

Por eso, buscar la oración completa en el archivo no encontrará una línea idéntica. La etiqueta del material es compartida entre misiones: `items_commodities_aluminum=Aluminio (RS 4285,8570,12855,17140,21425,25710)` puede reutilizarse en cualquier objetivo que incluya Aluminio. Si `(RS ...)` aparece en otra misión, es el resultado esperado de insertar esa misma etiqueta; no indica un fallo. El progreso, la cantidad y el destino pueden cambiar, mientras que el nombre del material y su RS proceden de la etiqueta compartida.

---

<a id="instalacion"></a>
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

<a id="contenido"></a>
## ✅ ¿Qué incluye?

### Versión ES (Español de España)

| Sistema | Estado | Notas |
|---------|--------|-------|
| Interfaz de usuario (UI) | ✅ Traducido | Menús, HUD, pantallas, etiquetas |
| Misiones y contratos | ✅ Traducido | Títulos, detalles, reputación, recompensas |
| Minería y materias primas | ✅ Traducido | Firmas de escaneo, ubicaciones y materiales |
| Fabricación y recetas | ✅ Traducido | Recetas, componentes y materiales |
| Ítems y equipamiento | ✅ Traducido | Armas, armaduras, escudos, motores |
| Pinturas de naves (Paint_*) | ✅ Traducido | Todas las claves de pintura traducidas |
| RS (firmas de escaneo de minería) | ✅ Añadido | Datos RS para los 26 tipos de mineral minable |
| Stanton | ✅ Traducido | Planetas, estaciones, ubicaciones y descripciones |
| Pantalla de energía de nave | ✅ Traducido | `hud_Label_Offline`, `engineering_ui_Item_Output`, etc. |

### Versión EN (Inglés Mejorado)

| Sistema | Estado | Notas |
|---------|--------|-------|
| Interfaz de usuario (UI) | ✅ Inglés original | Todos los textos en inglés |
| Datos RS (minería) | ✅ Añadidos | Valores RS para los 26 tipos de mineral minable |
| Firmas de escaneo / datos de minería | ✅ Fusionados | Desde enhancement INIs (DataForge XML) |
| Estadísticas de objetos y componentes | ✅ Integradas | `components_desc_enhancements.ini`, `ships_desc_enhancements.ini`, `ship_weapons_desc_enhancements.ini`, `fps_weapons_desc_enhancements.ini`, `missile_enhancements.ini` |
| Planos y materiales de fabricación | ✅ Fusionados | `commodity_crafting_enhancements.ini` |
| Consumibles médicos | ✅ Fusionados | `medical_consumables_enhancements.ini` |
| Diario | ✅ Fusionado | `journal_enhancements.ini` |
| Recompensas de misión | ✅ Fusionadas | `mission_rewards_enhancements.ini` |

---

<a id="mejoras-tecnicas"></a>
## 🛠 Mejoras técnicas aplicadas

### RS (Resource Signature) en minería
Se añadieron datos RS a las 26 claves `mineabletype_primary_*` (agricium, aluminium, aslarite, beryl, bexalite, borase, copper, corundum, gold, hephaestanite, ice, iron, laranite, lindinium, ouratite, quantainium, quartz, riccite, savrillium, silicon, stileron, taranite, tin, titanium, torite y tungsten). También se actualizaron las etiquetas de materias primas que reutilizan distintas interfaces. Consulta las capturas de la galería para ver ejemplos.

### Pantalla de energía de nave
Se añadió `hud_Label_Offline` y se corrigió `engineering_ui_Item_Output` para que aparezcan correctamente en la interfaz de gestión de energía de la nave.

### Archivos de mejoras integrados (versión EN)
Se integraron 9 archivos de mejoras generados a partir de datos DataForge extraídos de `Data.p4k` con `unp4k`:
- `commodity_crafting_enhancements.ini` — materiales y datos de fabricación
- `components_desc_enhancements.ini` — estadísticas de componentes de nave
- `ships_desc_enhancements.ini` — descripciones de naves
- `ship_weapons_desc_enhancements.ini` — armas de nave
- `fps_weapons_desc_enhancements.ini` — armas FPS
- `missile_enhancements.ini` — misiles
- `medical_consumables_enhancements.ini` — consumibles médicos
- `journal_enhancements.ini` — diario
- `mission_rewards_enhancements.ini` — recompensas de misión y planos

En total, se actualizaron **4.228 claves** entre las versiones ES y EN con datos de planos, estadísticas y materiales.

---

<a id="comunidad"></a>
## 🤝 Comunidad y soporte

Si vas a crear una cuenta nueva de Star Citizen, puedes usar mi código de referencia:

**STAR-6W9K-GDJB**

[Crear cuenta con el código de referencia](https://www.robertsspaceindustries.com/enlist?referral=STAR-6W9K-GDJB)

También puedes seguir las novedades o contactar con la comunidad:

- [Mi Discord](https://discord.gg/dAGHrr6K2f)
- [Canal de novedades del proyecto](https://discord.com/channels/283366132629504002/1567550721400770580)
- [Discord de la comunidad CCBE](https://discord.gg/8ZpvNM5qRB)
- [Web de CCBE](https://ccbe.space/)

---

<a id="errores"></a>
## 🐛 Errores y sugerencias

Si encuentras textos sin traducir, errores de ortografía o problemas de instalación, [abre un issue en GitHub](https://github.com/juniormaos-max/Star_citizen_traducion.ES/issues). También puedes avisar en el [canal de Discord para reportes](https://discord.com/channels/283366132629504002/1567541287601840328).

Al informar de un problema, incluye:
- Versión del juego (LIVE)
- Variante instalada (ES / EN)
- Captura de pantalla del error (si aplica)
- Texto original y texto esperado

---

<a id="creditos"></a>
## 🏆 Créditos

- **Proceso de traducción:** desarrollo propio con varias etapas de revisión (`rev1 → rev2 → rev3`)
- **Datos técnicos:** archivos DataForge de Star Citizen (fabricación, minería y materias primas)
- **Herramientas:** `unp4k` para extraer `Data.p4k`, además de `generate_enhancements_ini.py` y `gen_commodity_crafting.py` para generar archivos de mejoras
- **Imágenes y capturas:** aportes de la comunidad
- **Soporte:** comunidad CCBE y Discord

---

<a id="galeria"></a>
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

Las fichas de materiales incluyen ubicaciones y datos de planos (en qué se usan para fabricar).

![Minería en misiones](imagenes/mineria.png)
![Minería en misiones](imagenes/mineria1.png)
![Minería en misiones](imagenes/mineria2.png)
![Minería en misiones](imagenes/mineria3.png)

En algunas misiones de minería y de Battaglia, los objetivos muestran las firmas RS de los materiales minables.

![Minería en misiones](imagenes/newbabbage.png)

### Antes y después: ascensor de Levski (Nyx)

![Antes: el ascensor muestra el texto original](imagenes/levskiantes.png)

![Después: el ascensor muestra «ADUANAS»](imagenes/levskiahora.png)

En el ascensor de Levski, el texto **CUSTOMS** aparece traducido como **ADUANAS**.

![Aduana al salir del ascensor](imagenes/aduanaslesvki.png)

La señalización de la aduana al salir del ascensor también aparece en español.

### Criaturas de New Babbage

![Cuasi pastador de la tundra](imagenes/cuasi.png)

Criaturas en New Babbage: **CUASI PASTADOR DE LA TUNDRA**.

### Contratos: antes y después

![Contratos antes](imagenes/contratos_antes.png)

![Contratos ahora](imagenes/contratos_ahora.png)

En los contratos, la reputación (REP) aparece en los detalles de la misión, además de en el título.

### Refinerías y tiendas: antes y después

![Antes: pantalla de la refinería](imagenes/REFINARIA-ANTES.png)

![Después: pantalla de la refinería](imagenes/REFINARIA-AHORA.png)

![Antes: tienda de Levski](imagenes/TIENDA-ANTES.png)

![Después: tienda de Levski](imagenes/TIENDA-AHORA.png)

![Antes: pantalla de ASEC](imagenes/asce-antes.png)

![Después: pantalla de ASEC](imagenes/asce-ahora.png)

![Antes: tienda de ASEC](imagenes/asec1-antes.png)

![Después: tienda de ASEC](imagenes/asec1-ahora.png)

![Antes: tienda de minería](imagenes/mole-antes.png)

![Después: tienda de minería](imagenes/mole-ahora.png)

---

### Limitaciones conocidas

![Ejemplo de textos que no cambian con la localización](imagenes/LOL.png)

En las pruebas realizadas, estos textos no cambiaron al modificar sus entradas en `global.ini`. Por ahora, no se pueden traducir desde este paquete:

| Texto del juego | Clave de localización | Traducción prevista |
|---|---|---|
| `ORE SALES` | `shop_name_oresales` | Ventas de mineral |
| `TOUCH SCREEN TO START` | `med_Start_TouchScreenToBegin` | Toca la pantalla para comenzar |

---

*Última actualización: 14 de noviembre de 2026 — Star Citizen LIVE 4.10.3-REV 3.*

