# Reunión de validación con la cliente — 6 de noviembre de 2026

- **Modalidad:** Zoom, unos 60 minutos, en dos partes: requerimientos y prototipo.
- **Asistentes:** la Dra. Sara Ordóñez (cliente) y el equipo T6 – Los Guayabyte: Pablo Chacón, Jack Vera, William Pacalla y Fátima Torres.
- **Técnicas:**
  - validación de la priorización MoSCoW, módulo por módulo;
  - recorrido del prototipo navegable;
  - preguntas sobre los criterios de calidad.
- **Guion usado:** `Guion_Reunion_Validacion_NutriAgenda.pdf` (en esta carpeta).
- **Grabación:** se guarda como respaldo interno del equipo. No se publica en este repositorio.

## 1. Cambios de prioridad (MoSCoW)

| Módulo | Decisión de la doctora |
|---|---|
| Pacientes | Buscar y filtrar pacientes pasa a **Debe** («es lo básico»). |
| Historia clínica | Pasan a **Debe**: guardar el avance, subir exámenes y actualizar la historia en cada consulta. El recordatorio para llenarla se queda en **Debería**, con 2 envíos. |
| Agenda | Le gustó la lista de espera en el prototipo y se mantiene en **Debería**. El recordatorio de la cita es **Debe** («los pacientes no llegan»). |
| Mensajes | El agradecimiento después de la consulta va desde el inicio (**Debe**). Los correos salen desde su cuenta de **Outlook**. No se envían mensajes de noche ni en fin de semana. |
| Paquetes y pagos | Avisarle de cada cancelación desde el inicio (**Debe**). El plan dura 30 días y admite **una sola cancelación**. Si el paciente cancela tarde, cancela por segunda vez o no asiste, la consulta se considera tomada. Precios mencionados: consulta $50, a domicilio $70; quiere subirlos, por lo que se podrán configurar. |
| Reportes | Enviar el reporte por correo a cada médico pasa a **Debería**. El reporte se entrega al final del mes y lleva: nombre, fecha de atención, motivo, evolución, análisis antropométrico, exámenes, análisis y prescripción. |
| Seguridad | Todo lo de Debe y Debería lo quiere desde el inicio (**Debe**). |
| Won’t | Está de acuerdo con dejarlo para después. En el futuro le interesaría una app para que los pacientes registren comidas y síntomas. |
| Funciones sin módulo | Cumpleaños y mensajes motivacionales van a **Debería**. |

## 2. Funciones nuevas

- **Preparación para el análisis:** enviar las indicaciones a los pacientes de control (Debe).
- **Cálculos automáticos:** IMC y escalas de riesgo con los datos de la historia clínica (Podría).
- **Gráficos de evolución:** peso, grasa, masa muscular y lípidos (Podría).
- **Uso sin internet:** ver la información de los pacientes sin conexión (Debería).
- **Registro desde el computador:** registrar notas y mediciones en el panel web, porque trabaja en el computador durante la consulta.
- **Contacto directo:** botón «Prefiero escribir a la asistente por WhatsApp» para pacientes a quienes no les gusta la tecnología.

## 3. Observaciones al prototipo

La doctora lo aprobó: «Está súper bien, chicos, me gusta mucho». Pidió estos cambios:

- **Tono amable:** no usar la palabra «pierde»; usar «la consulta se considera tomada».
- **Lista de enfermedades:** cambiarla («la tiroides no es una condición»). Las opciones quedan así: diabetes, hipertensión, hipo o hipertiroidismo, colesterol o triglicéridos altos, enfermedad cardiovascular, otro trastorno hormonal o metabólico, otra y ninguna.
- **Agenda:** mostrar si el paciente es **nuevo** o de **control**.
- **Avisos:** quiere los de nuevas reservas y cancelaciones; **no** quiere el aviso de «historia clínica completada».
- **Letra grande:** «sí, claro, tengo muchos viejitos».
- **Outlook:** le parece importante, porque ahí tiene también su agenda personal (universidad, escuela de sus hijos); leer esos eventos para que no se crucen con las consultas sube a **Debe**.
- **Plataforma:** prefiere usar el sistema en el navegador del computador, donde trabaja con Outlook, y también desde el celular. La app móvil se reemplazó por un panel web con vista para computador y para celular.
- **Historia clínica:** se puede pedir al paciente que la actualice (por ejemplo, tras una cirugía).
- **Reporte para los médicos:** muestra motivo, evolución, análisis antropométrico, exámenes y análisis, y prescripción.

## 4. Valores de los criterios de calidad

| Criterio | Valor fijado |
|---|---|
| Reservar una cita | 2 minutos o menos |
| Llenar la historia clínica | 5 minutos o menos |
| Cambios en Outlook | Al minuto |
| Pérdida de datos aceptable | Ninguna (pidió copias de seguridad) |
| Mantenimiento | Las horas necesarias, de noche y preferiblemente en fin de semana |
| Bloqueo por inactividad | 15 minutos, con Face ID, sin perder lo que se estaba escribiendo |
| Mensajes fallidos | No más del 10 % |
| Vigencia de los enlaces | 72 horas |
| Capacidad | Máximo 4 pacientes por día |

## 5. Pendientes enviados por WhatsApp

Estos puntos no se alcanzaron a tratar en la reunión y se le enviaron por WhatsApp:

- nombre o iniciales del paciente en Outlook;
- herramienta para las videollamadas;
- descuento de cumpleaños, frecuencia de los mensajes motivacionales e «invitar a volver»;
- mensajes en fin de semana y horario exacto de atención;
- precios y cobro del plan;
- conservación de las historias clínicas;
- presupuesto y administración del sistema;
- permiso para entrevistar a la asistente y encuestar a pacientes;
- documentos actuales del consultorio.

La propuesta adoptada para cada uno está en la sección 9 del SRS.
