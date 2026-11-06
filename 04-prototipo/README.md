# Prototipo navegable

Tres archivos independientes, uno por usuario, que se abren en cualquier navegador:

| Archivo | Usuario | Pantallas |
|---|---|---|
| `paciente.html` | Paciente (enlace web en el celular) | P0 a P9 |
| `doctora.html` | Doctora (panel web: computador y celular; cambie la vista con los botones «Computador» y «Celular») | D1 a D10 |
| `asistente.html` | Asistente (panel web) | A0 a A8 |

Todos los botones tienen una acción: llevan a otra pantalla, cambian el estado de los datos ficticios o muestran lo que ocurriría en el sistema real (por ejemplo, abrir WhatsApp). El prototipo no guarda información; el botón «Reiniciar» lo deja como al inicio.

- `capturas/`: una imagen por pantalla, con el mismo código del SRS (P1, D2, A3…).
- `flujos/`: diagramas del flujo de ventanas de cada usuario.
