# ADR-[NÚMERO]: [Título de la Decisión]

**Fecha:** [YYYY-MM-DD]  
**Estado:** Propuesto | Aceptado | Deprecado | Reemplazado por [ADR-XXX]

## Contexto

[Describir el contexto y el problema que requiere una decisión. ¿Qué fuerzas están en juego? ¿Cuáles son las restricciones técnicas, de negocio o de equipo?]

Ejemplo:

> Nuestro sistema necesita almacenar datos de usuarios y libros. Debemos decidir qué tipo de base de datos utilizar considerando que el equipo tiene experiencia limitada en NoSQL y el proyecto tiene restricciones de tiempo.

## Decisión

[Describir la decisión tomada de manera clara y concisa]

Ejemplo:

> Utilizaremos PostgreSQL como base de datos relacional principal para el almacenamiento persistente.

## Opciones Consideradas

### Opción 1: [Nombre de la opción]

**Descripción:** [Breve descripción]

**Pros:**

- [Ventaja 1]
- [Ventaja 2]

**Contras:**

- [Desventaja 1]
- [Desventaja 2]

### Opción 2: [Nombre de la opción]

**Descripción:** [Breve descripción]

**Pros:**

- [Ventaja 1]
- [Ventaja 2]

**Contras:**

- [Desventaja 1]
- [Desventaja 2]

### Opción 3: [Nombre de la opción] ✓ SELECCIONADA

**Descripción:** [Breve descripción]

**Pros:**

- [Ventaja 1]
- [Ventaja 2]

**Contras:**

- [Desventaja 1]
- [Desventaja 2]

## Justificación

[Explicar por qué se eligió esta opción sobre las demás]

Ejemplo:

> Elegimos PostgreSQL porque:
>
> 1. El equipo tiene experiencia previa con bases de datos SQL
> 2. Los datos tienen relaciones claras (libros-préstamos-usuarios)
> 3. Necesitamos transacciones ACID para operaciones críticas
> 4. Es una solución probada y estable con amplia comunidad

## Consecuencias

### Positivas

- [Consecuencia positiva 1]
- [Consecuencia positiva 2]
- [Consecuencia positiva 3]

### Negativas

- [Consecuencia negativa 1]
- [Consecuencia negativa 2]

### Neutras

- [Consecuencia neutra 1]

## Riesgos

| Riesgo     | Probabilidad    | Impacto         | Mitigación |
| ---------- | --------------- | --------------- | ---------- |
| [Riesgo 1] | Alta/Media/Baja | Alto/Medio/Bajo | [Acción]   |
| [Riesgo 2] | Alta/Media/Baja | Alto/Medio/Bajo | [Acción]   |

## Métricas de Éxito

[¿Cómo sabremos si esta decisión fue correcta?]

- [ ] [Métrica 1]
- [ ] [Métrica 2]

## Referencias

- [Enlace a documentación relevante]
- [Enlace a discusiones relacionadas]
- [Enlace a ADRs relacionados]

## Notas

[Cualquier información adicional relevante]

---

## Historial de Cambios

| Fecha   | Autor   | Cambio                   |
| ------- | ------- | ------------------------ |
| [Fecha] | [Autor] | Creación inicial         |
| [Fecha] | [Autor] | [Descripción del cambio] |
