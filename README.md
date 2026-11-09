# Atención en taquilla · Farmacias CESAC

Página para contar los pacientes atendidos y las unidades entregadas en la taquilla de farmacia, a partir del reporte de remitos de SIGEHOS (módulo Medicación e insumos).

## Cómo se usa

1. En SIGEHOS, exportá el reporte de movimientos de fármacos e insumos **sin agrupar** (se descarga como `rptEstRemitos.xlsx`).
2. Abrí la página y cargá el Excel.
3. Elegí el período y, si querés pacientes por hora, cargá el horario de atención de cada día.

El Excel se procesa en el navegador: no se sube a ningún servidor ni se guarda. No hace falta instalar nada.

## Qué muestra

- Pacientes atendidos (atenciones con entrega efectiva) y pacientes distintos.
- Unidades de medicamentos y de descartables entregadas.
- Detalle por mes y por día, con copia de la tabla para Excel.
- Atención por día de la semana y pacientes por hora.
- Medicamentos más entregados y atenciones por dispensador.

## Criterios de conteo

- Solo remitos de tipo EGRESO, en estado CONFIRMADO, con paciente y cantidad mayor a cero.
- Los remitos devueltos quedan ANULADOS en SIGEHOS y no se cuentan.
- Una atención es un paciente que recibió al menos un producto en el día.
