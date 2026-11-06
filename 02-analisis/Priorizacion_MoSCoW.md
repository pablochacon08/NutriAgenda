# Priorización MoSCoW de los requerimientos funcionales

Priorización de los 80 requerimientos funcionales de NutriAgenda, **validada con la doctora en la reunión del 6 de noviembre de 2026** (fuente V1). Las demás fuentes son los códigos de las preguntas respondidas por ella en la guía (carpeta 01-levantamiento).

| Prioridad | Significado | Cantidad |
|---|---|---|
| Debe (Must) | Imprescindible para la primera entrega | 50 |
| Debería (Should) | Importante; puede ir en la segunda iteración | 23 |
| Podría (Could) | Deseable si hay tiempo | 7 |
| No por ahora (Won’t) | Fuera del alcance: API de WhatsApp Business, app para pacientes (incluido el registro de comidas y síntomas), cobro en línea, facturación del SRI, agenda de la segunda doctora | — |

## Debe (Must)

| ID | Módulo | Requerimiento | Fuente |
|---|---|---|---|
| RF-01 | M1. Gestión de pacientes | El sistema deberá permitir a la asistente o a la doctora registrar un paciente con nombres y apellidos, cédula (o pasaporte si es extranjero), fecha de nacimiento, número de WhatsApp, correo, ocupación, seguro médico (si tiene y cuál), tipo de paciente y, si es derivado, el médico derivador y su contacto. | B1, B13, D22 |
| RF-02 | M1. Gestión de pacientes | El sistema deberá identificar a cada paciente por su cédula y su nombre, e impedir registros duplicados. | B3 |
| RF-03 | M1. Gestión de pacientes | El sistema deberá permitir registrar pacientes menores de edad junto con los datos de su representante (nombre y cédula). | B3, H12 |
| RF-04 | M1. Gestión de pacientes | El sistema deberá clasificar a cada paciente como propio o derivado, y como paciente con plan mensual o por consulta. | B4, F2 |
| RF-05 | M1. Gestión de pacientes | El sistema deberá mostrar la ficha del paciente con la próxima cita en primer lugar, seguida de sus últimas mediciones y sus datos generales. | B5 |
| RF-06 | M1. Gestión de pacientes | El sistema deberá guardar en la historia del paciente el historial de consultas, las mediciones (peso, porcentaje de grasa y masa muscular) y las notas de evolución de la doctora. | B6 |
| RF-07 | M1. Gestión de pacientes | El sistema deberá permitir adjuntar y visualizar en la historia clínica los reportes PDF del equipo InBody y los exámenes de laboratorio. | B6, B8 |
| RF-08 | M1. Gestión de pacientes | El sistema deberá permitir buscar pacientes por nombre o cédula y filtrarlos por activos, derivados, propios y archivados. | B9, V1 |
| RF-12 | M1. Gestión de pacientes | El sistema deberá dar a la doctora y a la asistente acceso de lectura y edición a toda la información de los pacientes, desde la aplicación móvil o desde el panel web, porque la doctora registra las notas en el computador durante la consulta. | B10, H1, V1 |
| RF-13 | M2. Formularios e historia clínica | El sistema deberá presentar al paciente, desde un enlace, el formulario de historia clínica en cuatro pasos: datos personales y seguro; antecedentes y hábitos; alimentación habitual; y exámenes y consentimiento. El formulario es el mismo para todos los pacientes; en antecedentes, las enfermedades se eligen de una lista (hipertensión, diabetes, hipo o hipertiroidismo, colesterol o triglicéridos altos, enfermedad cardiovascular, otro trastorno hormonal o metabólico, otra o ninguna). | B2, C2, C4, V1 |
| RF-14 | M2. Formularios e historia clínica | El sistema deberá guardar automáticamente el avance del formulario para que el paciente pueda continuarlo después con el mismo enlace, mientras este siga vigente. | C5, V1 |
| RF-15 | M2. Formularios e historia clínica | El sistema deberá marcar la historia clínica como «completa» cuando todos los campos obligatorios estén llenos, y como «pendiente» en caso contrario, y mostrar ese estado en la agenda y en Outlook Calendar. | C6, C12, D11 |
| RF-16 | M2. Formularios e historia clínica | El sistema deberá permitir que el paciente suba exámenes de laboratorio en PDF o en imagen dentro del formulario. | C8, V1 |
| RF-17 | M2. Formularios e historia clínica | El sistema deberá exigir que el paciente, o su representante si es menor de edad, acepte el consentimiento de tratamiento de datos antes de enviar el formulario, y deberá guardar la fecha y la hora de la aceptación. | H5, H12 |
| RF-18 | M2. Formularios e historia clínica | El sistema deberá impedir que el paciente modifique el formulario una vez enviado y permitir que la asistente lo edite, registrando el cambio. | C9, H3 |
| RF-20 | M2. Formularios e historia clínica | El sistema deberá permitir actualizar la historia clínica en cada consulta y que el personal habilite un nuevo llenado del formulario cuando el paciente tenga cambios importantes (por ejemplo, una cirugía reciente). | C10, H3, V1 |
| RF-22 | M3. Citas, agenda y Outlook Calendar | El sistema deberá permitir configurar los horarios de atención de lunes a sábado (por la tarde de lunes a viernes y hasta el mediodía los sábados) y la duración de las consultas, de 30 a 45 minutos y hasta 60 minutos en casos especiales. | A7, A8, D1, D2 |
| RF-23 | M3. Citas, agenda y Outlook Calendar | El sistema deberá permitir que la asistente registre feriados, vacaciones y días bloqueados, en los que no se ofrecen horarios. | D15 |
| RF-24 | M3. Citas, agenda y Outlook Calendar | El sistema deberá permitir que el paciente reserve una cita desde su enlace, eligiendo la modalidad (presencial o virtual), el día y una hora entre los horarios disponibles, incluido el mismo día si hay disponibilidad. | D3, D4, D5 |
| RF-26 | M3. Citas, agenda y Outlook Calendar | El sistema deberá permitir que el paciente con plan mensual elija las fechas de sus dos consultas del mes, separadas aproximadamente 15 días, y registrar como «tomadas» las consultas que no use dentro de los 30 días del plan. | D10, D20, F2, V1 |
| RF-27 | M3. Citas, agenda y Outlook Calendar | El sistema deberá permitir que el paciente confirme su asistencia desde el enlace hasta el día anterior a la cita. | D7 |
| RF-28 | M3. Citas, agenda y Outlook Calendar | El sistema deberá permitir que el paciente reprograme una cita una sola vez, con anticipación, sin que cuente como cancelación. | D8, F4 |
| RF-29 | M3. Citas, agenda y Outlook Calendar | El sistema deberá permitir que el paciente cancele una cita hasta un día antes, previa confirmación, sin liberar automáticamente el horario. | D8, D9 |
| RF-31 | M3. Citas, agenda y Outlook Calendar | El sistema deberá manejar los estados de cita «por confirmar», «confirmada», «cancelada», «atendida» y «no asistió», y permitir que la asistente y la doctora los cambien. | D6 |
| RF-32 | M3. Citas, agenda y Outlook Calendar | El sistema deberá permitir que el personal agende, mueva o cancele citas en nombre del paciente cuando este lo solicite. | D14 |
| RF-33 | M3. Citas, agenda y Outlook Calendar | El sistema deberá mostrar a la doctora y a la asistente la agenda en vista de semana y de lista, con el nombre del paciente, la hora, si es paciente nuevo o de control, el estado de la cita y el estado de la historia clínica. | D17, C12, V1 |
| RF-34 | M3. Citas, agenda y Outlook Calendar | El sistema deberá sincronizar con el Outlook Calendar personal de la doctora las citas confirmadas y pendientes, con el nombre del paciente (o solo sus iniciales, según decida la doctora) y el estado de su historia clínica. | D11, V1 |
| RF-40 | M4. Mensajería | El sistema deberá enviar automáticamente por correo, al momento de agendar, el mensaje de bienvenida con las políticas del programa y el enlace de la historia clínica. | E2, E5 |
| RF-41 | M4. Mensajería | El sistema deberá generar, 3 días antes de la cita, el mensaje para que el paciente confirme su asistencia. | E2, D7 |
| RF-42 | M4. Mensajería | El sistema deberá generar, 1 día antes de la cita, el mensaje con el código QR de acceso al edificio. | A10, E2 |
| RF-43 | M4. Mensajería | El sistema deberá enviar recordatorios de la cita 24 horas y 3 horas antes. | E3, V1 |
| RF-44 | M4. Mensajería | El sistema deberá preparar cada mensaje de WhatsApp con el texto ya escrito y abrir WhatsApp Web o la aplicación del iPhone, para que la asistente o la doctora lo envíen; luego deberá marcarlo como enviado. | E7, E8, E10 |
| RF-45 | M4. Mensajería | El sistema deberá enviar los correos desde la cuenta de correo de Outlook de la doctora, que es la que ella maneja, con la opción de cambiarla por un correo con dominio propio. | E4, E6, V1 |
| RF-46 | M4. Mensajería | El sistema deberá enviar, después de la consulta, un mensaje de agradecimiento con el reporte InBody adjunto. | E12, E15, V1 |
| RF-49 | M4. Mensajería | El sistema solo deberá enviar o dejar listos mensajes de lunes a viernes, en la mañana y la tarde; los envíos que caigan de noche o en fin de semana se adelantarán al último horario hábil anterior. | E18, V1 |
| RF-74 | M4. Mensajería | El sistema deberá enviar a los pacientes de las consultas de control las indicaciones de preparación para el análisis de composición corporal. | V1 |
| RF-51 | M5. Paquetes, pagos y cancelaciones | El sistema deberá registrar el plan mensual de cada paciente (2 consultas por $70, con vigencia de 30 días) y llevar la cuenta de las consultas usadas, pendientes y tomadas sin asistir. | F1, F2, V1 |
| RF-52 | M5. Paquetes, pagos y cancelaciones | El sistema deberá registrar los pagos completos de planes y de consultas individuales, con monto, fecha y método (efectivo o transferencia). | F6, F7, F8 |
| RF-56 | M5. Paquetes, pagos y cancelaciones | El sistema deberá notificar a la doctora toda cancelación y toda reprogramación. | F12, V1 |
| RF-58 | M6. Reportes | El sistema deberá generar al final de cada mes el reporte de pacientes derivados, uno por cada médico derivador, con el nombre de cada paciente, las fechas de atención, el motivo de consulta, la evolución, el análisis antropométrico, los resultados de exámenes, el análisis, la prescripción y el estado del plan. | A11, G1, G6, V1 |
| RF-59 | M6. Reportes | El sistema deberá generar cada mes el reporte de los pacientes privados de la doctora. | G1 |
| RF-60 | M6. Reportes | Los reportes deberán incluir los ingresos del período y la cantidad de pacientes nuevos. | G1 |
| RF-62 | M6. Reportes | El sistema deberá exportar los reportes en PDF y en Excel. | G3, G7, G8 |
| RF-64 | M7. Seguridad y acceso | El sistema deberá exigir correo y contraseña en el primer inicio de sesión de cada dispositivo y luego permitir el ingreso rápido (Face ID en el iPhone), manteniendo la sesión abierta hasta un día, y bloquear la aplicación tras 15 minutos sin uso, sin perder lo que se estaba registrando. | H2, V1 |
| RF-65 | M7. Seguridad y acceso | El sistema deberá generar enlaces únicos para los pacientes, con validez máxima de 72 horas, y desactivar el enlace del formulario una vez enviado. | H3 |
| RF-67 | M7. Seguridad y acceso | El sistema deberá pedir un código de verificación enviado al correo para los cambios importantes: editar el formulario, dar o quitar accesos y eliminar datos. | H14, V1 |
| RF-68 | M7. Seguridad y acceso | El sistema deberá permitir cerrar la sesión a distancia en todos los dispositivos. | H9, V1 |
| RF-69 | M7. Seguridad y acceso | El sistema deberá permitir crear la cuenta de la asistente y darle o quitarle el acceso. | H15 |
| RF-70 | M7. Seguridad y acceso | El sistema deberá registrar quién consultó o modificó una ficha, una cita o un pago, y cuándo. | H10, V1 |
| RF-71 | M7. Seguridad y acceso | El sistema deberá eliminar todos los datos de un paciente cuando este lo solicite. | H6 |

## Debería (Should)

| ID | Módulo | Requerimiento | Fuente |
|---|---|---|---|
| RF-09 | M1. Gestión de pacientes | El sistema deberá permitir archivar y reactivar a un paciente; los pacientes archivados no aparecen en la lista activa ni pueden agendar citas. | B11 |
| RF-11 | M1. Gestión de pacientes | El sistema deberá permitir la carga inicial manual, desde el panel web, de los pacientes que hoy están en Word y Excel (alrededor de 10). | B12 |
| RF-72 | M1. Gestión de pacientes | El sistema deberá permitir que la doctora consulte en su aplicación la agenda y las fichas de los pacientes sin conexión a internet, con los datos de la última sincronización, y enviar al reconectarse lo que haya registrado sin conexión. | V1 |
| RF-19 | M2. Formularios e historia clínica | El sistema deberá generar hasta dos recordatorios para el paciente que no haya llenado su historia clínica, sin reprogramar su cita. | C7, V1 |
| RF-21 | M2. Formularios e historia clínica | El sistema deberá permitir que la doctora agregue, quite y modifique las preguntas del formulario, e indique si cada una es obligatoria u opcional, sin ayuda técnica. | C13 |
| RF-25 | M3. Citas, agenda y Outlook Calendar | El sistema deberá limitar a dos el número de citas futuras de un mismo paciente. | D16 |
| RF-30 | M3. Citas, agenda y Outlook Calendar | El sistema deberá mantener una lista de espera en la que se anoten los pacientes, y permitir que la asistente ofrezca un horario cancelado a una persona de la lista. | D9, V1 |
| RF-35 | M3. Citas, agenda y Outlook Calendar | El sistema deberá leer los eventos personales del Outlook Calendar de la doctora y bloquear esos horarios para los pacientes. | D12, D13 |
| RF-36 | M3. Citas, agenda y Outlook Calendar | El sistema deberá permitir que la doctora bloquee horarios de su agenda personal desde la aplicación móvil. | D13 |
| RF-37 | M3. Citas, agenda y Outlook Calendar | El sistema deberá permitir registrar el enlace de la videollamada de las citas virtuales (Zoom u otra herramienta que indique la doctora) e incluirlo en el evento de Outlook y en los mensajes al paciente. | D5 |
| RF-38 | M3. Citas, agenda y Outlook Calendar | El sistema deberá permitir marcar una cita como «no asistió», o reprogramarla, cuando el paciente supere los 15 minutos de tolerancia; si el paciente tiene plan, la consulta se registra como tomada. | D18, V1 |
| RF-47 | M4. Mensajería | El sistema deberá registrar el historial de mensajes de cada paciente, con la fecha, el canal y el estado (enviado o fallido). | E13 |
| RF-48 | M4. Mensajería | El sistema deberá permitir editar las plantillas de los mensajes y usar campos automáticos como nombre, fecha, hora y enlace, con trato de «usted» y emojis. | E9, E14 |
| RF-50 | M4. Mensajería | El sistema deberá reintentar automáticamente el envío de un correo que falle y avisar a la asistente si no lo logra. | R7 (taller) |
| RF-75 | M4. Mensajería | El sistema deberá generar el mensaje de felicitación el día del cumpleaños de cada paciente activo. | Hechos del cliente, V1 |
| RF-76 | M4. Mensajería | El sistema deberá generar mensajes motivacionales periódicos para los pacientes activos, con una frecuencia configurable. | Hechos del cliente, V1 |
| RF-78 | M4. Mensajería | El sistema deberá mostrar en las pantallas del paciente un botón para escribir directamente a la asistente por WhatsApp, para quienes prefieran no usar el sistema. | V1 |
| RF-53 | M5. Paquetes, pagos y cancelaciones | El sistema deberá marcar como «por renovar» el plan que haya usado todas sus consultas, y permitir renovarlo al registrar un nuevo pago. | F5, F10 |
| RF-54 | M5. Paquetes, pagos y cancelaciones | El sistema deberá permitir que la doctora apruebe o rechace excepciones a las reglas del plan, como recuperar una consulta que se dio por tomada. | F5 |
| RF-55 | M5. Paquetes, pagos y cancelaciones | El sistema deberá mostrar al paciente, desde su enlace, el estado de las consultas de su plan. | F11 |
| RF-57 | M5. Paquetes, pagos y cancelaciones | El sistema deberá informar al médico derivador cuando uno de sus pacientes cancele o abandone el plan. | F13 |
| RF-61 | M6. Reportes | El sistema deberá permitir filtrar los reportes por rango de fechas. | G5 |
| RF-63 | M6. Reportes | El sistema deberá permitir enviar por correo a cada médico derivador su reporte. | G2, G6, V1 |

## Podría (Could)

| ID | Módulo | Requerimiento | Fuente |
|---|---|---|---|
| RF-10 | M1. Gestión de pacientes | El sistema deberá permitir agregar etiquetas y notas libres a cada paciente. | B14 |
| RF-73 | M2. Formularios e historia clínica | El sistema deberá calcular automáticamente, con los datos de la historia clínica y las mediciones, el índice de masa corporal y las escalas de riesgo que defina la doctora (por ejemplo, riesgo cardiovascular). | V1 |
| RF-39 | M3. Citas, agenda y Outlook Calendar | El sistema deberá mostrar a los pacientes que están en el extranjero la hora de la cita virtual en la zona horaria de su dispositivo, además de la hora de Ecuador. | D22 |
| RF-79 | M3. Citas, agenda y Outlook Calendar | El sistema deberá presentar al paciente nuevo, antes de reservar, un cuestionario corto de filtro (primera consulta, médico que lo deriva y motivo principal). | Hechos del cliente, V1 |
| RF-77 | M4. Mensajería | El sistema deberá invitar a volver a los pacientes que lleven un tiempo configurable sin cita. | Hechos del cliente |
| RF-80 | M6. Reportes | El sistema deberá mostrar gráficos de la evolución del paciente (peso, porcentaje de grasa, masa muscular y resultados de exámenes como los lípidos) en la ficha y en el reporte. | V1 |
| RF-66 | M7. Seguridad y acceso | El sistema deberá poder solicitar el número de cédula al abrir el formulario, para confirmar la identidad del paciente. | H4 |
