# Casos de uso - Sistemas de Gestion Hospitalaria 

## Actores
- Recepcionista 
- Medico
- Administrador 
- Paciente

---

## CU-01: Registrar Paciente 

**Actor:** Recepcionista 
**Descripcion:** Permite registrar un nuevo paciente en el sistema.

**Flujo Principall:**
1. El recepcionista ingresa los datos personales del paciente.
2. Ingresa el historial clinico y grupo sanguineo.
3. Registrar alergias y contraindicaciones.
4. El sistema valida la informacion.
5. El sistema guarda el paciente.

**flujos alternos:**
- Datos invalidos → El sistema muestra error.

---

## CU-02: Agendar Cita Medica 

**Actor:** Recepcionsta 

**Flujo principal:**
1. Selecciona paciente.
2. Selecciona medico.
3. Ingresa fecha y hora.
4. El sistema valida disponibilidad.
4. Se registrar la cita con estado "PENDIENTE".

**Flujo alternos:**
- Medico no disponible → Se rechaza la cita.

## CU-03: Atender Paciente

**Actor:** Medico

**Flujo Principal:**
1. El medico selecciona la cita.
2. Cambia el estado a "EN_ATENCION".
3. Registra diagnostico.
4. Marca la cita como "COMPLETADA".