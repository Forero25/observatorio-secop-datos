# observatorio-secop-datos

CSV agregados del [Observatorio de contratación pública](https://nicolasforero.pages.dev) que alimentan el tablero de Power BI. Se reemplazan cada día en el release [`datos`](https://github.com/Forero25/observatorio-secop-datos/releases/tag/datos).

Los genera el pipeline del observatorio (ingesta de SECOP II, modelos en dbt y pronóstico en R) y los sube aquí su flujo diario. Este repositorio no tiene código: solo los datos publicados.

## Qué hay

| Archivo | Contenido |
|---|---|
| `hechos_contratos.csv` | Conteo y valor de contratos por mes, municipio, tipo de entidad, modalidad, tipo de contrato y tipo de proveedor |
| `municipio_anio.csv` | Proveedores distintos y concentración (HHI) por municipio y año |
| `serie_mensual.csv` | Contratos firmados por mes en todo el país |
| `pronostico*.csv` | Pronóstico de los próximos 12 meses, su evaluación retrospectiva y el resumen del modelo |
| `calendario.csv`, `territorio.csv`, `entidad.csv`, `modalidad.csv`, `tipo_contrato.csv` | Dimensiones |
| `rangos.csv`, `metadatos.csv` | Rangos de referencia y fecha de corte |

Ningún archivo trae nombres, documentos ni seudónimos de contratistas: solo conteos agregados.

## Fuente y licencia

Datos de [SECOP II - Contratos Electrónicos](https://www.datos.gov.co/Gastos-Gubernamentales/SECOP-II-Contratos-Electr-nicos/jbjy-vk9h), publicados por la Agencia Nacional de Contratación Pública – Colombia Compra Eficiente en datos.gov.co bajo licencia CC BY-SA 4.0. Estos agregados son una obra derivada y se comparten con la misma licencia ([LICENSE](LICENSE)).

Los indicadores son señales estadísticas para orientar la revisión, no acusaciones contra entidades ni personas.
