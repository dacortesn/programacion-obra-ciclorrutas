# Seguimiento a la programación de obra – Ciclorrutas Sabana

Tablero de seguimiento a la programación del contratista de las ciclorrutas de la Sabana (ICCU, CTO 1246/2023): avance programado frente a la línea base, avance reportado por frente, subtramos en espera de predios, cronograma, hitos y actividades del periodo, con un mapa de subtramos sobre los ejes del proyecto.

- **Programación:** `261105 ICCU 1246 de 2023 - PROGRAMACIÓN DE OBRA V0_LB.1.mpp` (MS Project), exportada e incrustada en la página. Trae la línea base y la programación vigente; no trae avance real.
- **Avance reportado y estado predial:** hoja «FRENTES DE OBRA 2026», leída en vivo cada vez que se abre la página y cruzada por abscisa con cada subtramo. Si no responde, se usa un corte guardado y la página lo avisa. La hoja debe seguir compartida como «cualquier persona con el enlace puede ver».
- **Ejes y predios:** los mismos de los tableros predial y ambiental (PROYECTO CICLORUTAS.kmz, IGAC).

La página abre en la **semana en curso**: el mapa (primera sección) resalta los subtramos con obra programada esa semana, coloreados por actividad, y debajo se listan las actividades por tramo y abscisa con alertas frente a la hoja de frentes. Con las flechas se recorre cualquiera de las semanas del programa. La fecha de corte de los indicadores se puede cambiar; por defecto es el día en que se abre.

Todo el sitio es un solo archivo, `index.html`. Si llega una nueva versión del MPP, hay que exportarla y regenerar el sitio:

```
.\scripts\exportar_mpp.ps1 -Mpp 'ruta\nueva programación.mpp'
.\scripts\construir_sitio.ps1
```
