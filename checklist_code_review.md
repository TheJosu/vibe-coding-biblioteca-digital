# Checklist de Code Review

## Información del Review

| Campo        | Valor                      |
| ------------ | -------------------------- |
| **PR/MR**    | #[número]                  |
| **Autor**    | [nombre]                   |
| **Reviewer** | [nombre]                   |
| **Fecha**    | [fecha]                    |
| **Branch**   | feature/[nombre] → develop |

---

## 1. Funcionalidad

- [ ] El código hace lo que se espera según los requisitos
- [ ] Los casos edge están manejados
- [ ] El código maneja errores correctamente
- [ ] No hay regresiones en funcionalidad existente

**Comentarios:**

```
[Escribir comentarios aquí]
```

---

## 2. Diseño y Arquitectura

- [ ] El código sigue la arquitectura del proyecto
- [ ] Las responsabilidades están bien separadas (SRP)
- [ ] No hay código duplicado (DRY)
- [ ] Las abstracciones son apropiadas
- [ ] Los patrones de diseño se usan correctamente
- [ ] Las dependencias están bien manejadas (DIP)

**Comentarios:**

```
[Escribir comentarios aquí]
```

---

## 3. Código Limpio

### Nomenclatura

- [ ] Los nombres de variables son descriptivos
- [ ] Los nombres de funciones indican qué hacen
- [ ] Los nombres de clases son sustantivos
- [ ] No hay abreviaturas ambiguas
- [ ] Convención de nombres consistente (camelCase, snake_case, etc.)

### Funciones

- [ ] Las funciones son pequeñas (< 20 líneas ideal)
- [ ] Cada función hace una sola cosa
- [ ] Pocos parámetros (< 4 ideal)
- [ ] Sin efectos secundarios inesperados

### Comentarios

- [ ] El código es autoexplicativo (mínimos comentarios necesarios)
- [ ] Los comentarios explican "por qué", no "qué"
- [ ] No hay código comentado sin explicación
- [ ] JSDoc/docstrings en funciones públicas

**Comentarios:**

```
[Escribir comentarios aquí]
```

---

## 4. Complejidad

- [ ] La lógica es fácil de seguir
- [ ] No hay anidamiento excesivo (< 3 niveles)
- [ ] No hay funciones demasiado largas
- [ ] La complejidad ciclomática es razonable
- [ ] Se puede entender sin necesidad del autor

**Comentarios:**

```
[Escribir comentarios aquí]
```

---

## 5. Testing

- [ ] Hay tests para la nueva funcionalidad
- [ ] Los tests cubren casos positivos
- [ ] Los tests cubren casos de error
- [ ] Los tests cubren casos edge
- [ ] Los tests siguen AAA (Arrange, Act, Assert)
- [ ] Los tests son independientes
- [ ] No hay tests flaky (inestables)
- [ ] La cobertura es adecuada (> 80%)

**Comentarios:**

```
[Escribir comentarios aquí]
```

---

## 6. Seguridad

- [ ] No hay credenciales hardcodeadas
- [ ] Los inputs están validados
- [ ] No hay vulnerabilidades de inyección (SQL, XSS, etc.)
- [ ] Los datos sensibles están protegidos
- [ ] Las contraseñas se hashean correctamente
- [ ] No hay información sensible en logs

**Comentarios:**

```
[Escribir comentarios aquí]
```

---

## 7. Rendimiento

- [ ] No hay operaciones N+1 en base de datos
- [ ] No hay bucles innecesarios
- [ ] Los recursos se liberan correctamente
- [ ] No hay memory leaks potenciales
- [ ] Las consultas están optimizadas
- [ ] Se usa caching donde es apropiado

**Comentarios:**

```
[Escribir comentarios aquí]
```

---

## 8. Mantenibilidad

- [ ] El código es fácil de modificar
- [ ] Las configuraciones están externalizadas
- [ ] Los magic numbers están como constantes
- [ ] El código es extensible sin modificación (OCP)
- [ ] Hay separación clara de concerns

**Comentarios:**

```
[Escribir comentarios aquí]
```

---

## 9. Estilo y Formato

- [ ] El código pasa el linter
- [ ] El formato es consistente
- [ ] Los imports están organizados
- [ ] No hay código muerto
- [ ] Archivos de tamaño razonable

**Comentarios:**

```
[Escribir comentarios aquí]
```

---

## 10. Documentación

- [ ] README actualizado si es necesario
- [ ] Cambios en API documentados
- [ ] Configuraciones nuevas documentadas
- [ ] Changelog actualizado

**Comentarios:**

```
[Escribir comentarios aquí]
```

---

## Resumen

### Resultado

- [ ] ✅ **Aprobado** - Sin cambios requeridos
- [ ] ⚠️ **Aprobado con comentarios** - Cambios menores opcionales
- [ ] 🔄 **Cambios requeridos** - Debe modificarse antes de merge
- [ ] ❌ **Rechazado** - Requiere rediseño significativo

### Puntos Positivos

1. [Punto positivo 1]
2. [Punto positivo 2]
3. [Punto positivo 3]

### Puntos a Mejorar

1. [Punto a mejorar 1]
2. [Punto a mejorar 2]
3. [Punto a mejorar 3]

### Comentarios Generales

```
[Comentarios finales del reviewer]
```

---

## Guía de Severidad para Comentarios

| Severidad         | Descripción                                   | Acción                          |
| ----------------- | --------------------------------------------- | ------------------------------- |
| 🔴 **Blocker**    | Bug crítico o vulnerabilidad                  | Debe corregirse antes del merge |
| 🟠 **Major**      | Problema importante de diseño o funcionalidad | Debe corregirse                 |
| 🟡 **Minor**      | Mejora de código o estilo                     | Recomendado corregir            |
| 🟢 **Suggestion** | Sugerencia opcional                           | A criterio del autor            |
| 💬 **Question**   | Pregunta o discusión                          | No bloquea                      |
| 👍 **Praise**     | Reconocimiento de buen código                 | N/A                             |

---

_Fecha del review: [fecha]_  
_Tiempo invertido: [X] minutos_
