# Caracterización GNSS+DInSAR del sismo de Venezuela (24 de junio de 2026)

**Rol:** Co-autora e investigadora responsable del procesamiento GNSS y de la integración GNSS+DInSAR.
**Institución:** Laboratorio de Geodesia Física y Satelital "Dr. Melvin Hoyer" (LGFS-MH), Departamento de Geodesia Superior, Escuela de Ingeniería Geodésica, Universidad del Zulia.
**Coautor:** Prof. Hermógenes David Suárez Acosta.

## Contexto
El 24 de junio de 2026, un doblete sísmico (Mw 7.2 y Mw 7.5, separados por ~39 s) afectó el centro-norte de Venezuela, al oeste de Caracas, en la zona de interacción entre las placas Caribe, Suramericana y el Bloque de los Andes del Norte. Se realizó una caracterización geodésica temprana de la deformación co-sísmica en dos etapas: primero solo con GNSS, y luego integrando GNSS con DInSAR.

## Metodología

**GNSS (estación CCS1, Caracas):**
- Procesamiento independiente por dos vías: CSRS-PPP (Natural Resources Canada) y OPUS (NOAA/NGS), en modo estático y cinemático.
- Sesiones de 24 h, muestreo cada 30 s, días 22–26 de junio de 2026; referencia ITRF2020 (época 2026.5).
- Ampliado luego a 7 estaciones regionales (REMOS/IGVSB y COCONet/GAGE) para contexto espacial.

**DInSAR (Sentinel-1):**
- 5 pares interferométricos (2 ascendentes, 3 descendentes), banda C, SLC, polarización VV, adquiridos entre el 6 y el 25 de junio de 2026.
- Procesamiento vía ASF HyP3 (hyp3_gamma 9.1.0 / GAMMA), 20 range looks × 4 azimuth looks, filtro adaptativo ADF=0.6, desenvolvimiento de fase por Minimum Cost Flow, DEM Copernicus GLO-30, geocodificación UTM 19N.

**Integración GNSS+DInSAR:**
- Ajuste por mínimos cuadrados ponderado combinando LOS ascendente/descendente con la restricción GNSS en CCS1 (Sentinel-1 tiene baja sensibilidad norte-sur, por lo que dN depende principalmente del GNSS).
- Análisis exploratorio en 20 puntos de interés (aeropuertos, autopistas, viaductos, túneles) entre Aragua, Carabobo, La Guaira, Miranda y Yaracuy.

## Resultados
- GNSS en CCS1 (fase 1): dE = −0.464 m, dN = −0.011 m, dU = +0.021 m.
- Solución GNSS+DInSAR restringida con CCS1 (fase 2): dE = −0.475 m, dN = −0.008 m, dU = +0.043 m.
- Desplazamiento horizontal en los 20 puntos de interés: 0.432–0.522 m (RMS ±0.482 m); vertical: 0.029–0.048 m (RMS ±0.038 m).
- Mayor desplazamiento en el corredor Caracas–La Guaira (autopista, viaducto y túneles Boquerón I y II).
- Resultados consistentes con productos independientes de ESA, JAXA y NASA/NISAR, y con el reporte GNSS de alta frecuencia de DIGA-UCV.

## Relevancia para gestión territorial
El estudio evidenció la necesidad de actualizar el marco de referencia geodésico nacional y el sistema de alturas (afectado cerca del mareógrafo de La Guaira), y recomendó ampliar la red REMOS y desplegar reflectores de esquina para monitoreo geodinámico continuo.

## Publicaciones relacionadas
- Arenas Bermúdez, I. y Suárez Acosta, H.D. (2026). *Evidencia GNSS preliminar de deformación co-sísmica en Caracas...* — [ES](https://siggma.xyz/evidencia-gnss-preliminar-terremoto-caracas/) | [EN](https://siggma.xyz/preliminary-gnss-evidence-earthquake-caracas/)
- Suárez Acosta, H.D. y Arenas Bermúdez, I. (2026). *Preliminary GNSS+DInSAR Evidence of Coseismic Deformation...* (reporte técnico completo) — [EN](https://siggma.xyz/preliminary-gnssdinsar-evidence-of-coseismic-deformation-in-caracas-la-guaira-associated-with-the-june-24-2026-earthquakes/)
- Suárez Acosta, H.D. y Arenas Bermúdez, I. (2026). *Geodesia: la ciencia que midió y reveló un desplazamiento de medio metro en Venezuela* (síntesis divulgativa) — [ES](https://siggma.xyz/geodesia-la-ciencia-que-midio-y-revelo-un-desplazamiento-de-medio-metro-en-venezuela/) | [EN](https://siggma.xyz/geodesy-the-science-that-measured-and-revealed-a-half-meter-displacement-in-venezuela/)

## Agradecimientos
ASF DAAC, NASA Earthdata Cloud, ESA/Copernicus (datos Sentinel-1 y procesamiento HyP3), IGVSB/REMOS y EarthScope/GAGE (datos GNSS), NRCan (CSRS-PPP), NOAA/NGS (OPUS), USGS (catálogo sísmico).
