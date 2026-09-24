# TRA-001 - Matriz de Trazabilidad de SoftEdu

## Información del elemento de configuración

- Código del CI: TRA-001
- Nombre: Matriz de Trazabilidad
- Proyecto: SoftEdu
- Versión: 1.1
- Estado: Aprobado
- Fecha: 23/09/2026
- Responsable: Equipo SoftEdu
- Responsable del cambio: SthephaniGP, mediante PR#3
  
## Historial de versiones
| Versión | Fecha | Descripción del cambio | Responsable |
|---------|-------|------------------------|-------------|
| 1.0 | 09/09/2026 | Creación inicial de la matriz de trazabilidad | Equipo SoftEdu |
| 1.1 | 16/09/2026 | Actualización de la trazabilidad asociada a CR-001 - Agregar teléfono al estudiante | SthephaniGP
|

## 1. Objetivo
Relacionar los requisitos definidos para SoftEdu con los elementos de diseño, código fuente y pruebas que los
implementan o verifican.
La matriz permite identificar qué elementos de configuración deben revisarse cuando un requisito sea modificado y
registrar la trazabilidad de las solicitudes de cambio.

## 2. Matriz de trazabilidad
| Requisito | Descripción | Diseño relacionado | Código relacionado | Prueba relacionada | Estado |
|-----------|-------------|--------------------|--------------------|--------------------|--------|
| RF-01 | Registrar estudiante | DIS-001 v1.1 - Entidad Estudiante | SRC-001 v1.1 - Gestión de Estudiantes | TST-001 v1.1 /
CP-01 | Completa |
| RF-02 | Consultar estudiante | DIS-001 - Entidad Estudiante | SRC-001 - Gestión de Estudiantes | TST-001 / CP-02 |
Completa |
| RF-03 | Registrar curso | DIS-001 - Entidad Curso | Pendiente de implementación | TST-001 / CP-03 | Parcial |
| RF-04 | Matricular estudiante | DIS-001 - Entidad Matrícula | Pendiente de implementación | TST-001 / CP-04 | Parcial |

## 3. Relación entre elementos de configuración afectados por CR-001
CR-001 - Agregar teléfono al estudiante
↓
REQ-001 v1.1 - RF-01 Registrar estudiante
↓
DIS-001 v1.1 - Entidad Estudiante
↓
SRC-001 v1.1 - Gestión de Estudiantes
↓
TST-001 v1.1 - CP-01 Registrar estudiante correctamente
↓
TRA-001 v1.1 - Actualización de la trazabilidad

## 4. Trazabilidad por requisito

### RF-01 - Registrar estudiante
- Requisito: REQ-001 v1.1
- Cambio asociado: CR-001 - Agregar teléfono al estudiante
- Diseño asociado: DIS-001 v1.1 - Entidad Estudiante
- Código asociado: SRC-001 v1.1 - Gestión de Estudiantes
- Caso de prueba asociado: TST-001 v1.1 / CP-01
- Estado de trazabilidad: Completa
- Estado del cambio: Aprobado e integrado por el main
- Responsable de integración y aprobación: erikaucp
- Commit de integración:7872add
  
### RF-02 - Consultar estudiante
- Requisito: REQ-001
- Diseño asociado: DIS-001 - Entidad Estudiante
- Código asociado: SRC-001 - Gestión de Estudiantes
- Caso de prueba asociado: TST-001 / CP-02
- Estado de trazabilidad: Completa
  
### RF-03 - Registrar curso
- Requisito: REQ-001
- Diseño asociado: DIS-001 - Entidad Curso
- Código asociado: Pendiente
- Caso de prueba asociado: TST-001 / CP-03
- Estado de trazabilidad: Parcial
  
### RF-04 - Matricular estudiante
- Requisito: REQ-001
- Diseño asociado: DIS-001 - Entidad Matrícula
- Código asociado: Pendiente
- Caso de prueba asociado: TST-001 / CP-04
- Estado de trazabilidad: Parcial
  
## 5. Trazabilidad de cambios
Solicitud de cambio CR-001
↓
RF-01 de REQ-001 v1.1
↓
DIS-001 v1.1
↓
SRC-001 v1.1
↓
TST-001 v1.1 / CP-01
↓
Commits asociados a CR-001
↓
Commits de corrección en el PR #2
↓
Commits de implementación incluidos en el PR #3
↓
PR #2 - Revisado y aprobado por erikaucp
↓
PR #3 - Revisado y aprobado por erikaucp
↓
Integrado en main - Commit 7872add

## 6. Registro de cambios trazables
| Solicitud de cambio | Requisito afectado | Diseño afectado | Código afectado | Prueba afectada | Commit / PR | Estado |
|--------------------|--------------------|-----------------|-----------------|-----------------|-------------|--------|
| Sin cambios aprobados en la versión 1.0 | - | - | - | - | - | Línea base inicial |
| CR-001 - Agregar teléfono al estudiante | REQ-001 v1.1 / RF-01 | DIS-001 v1.1 | SRC-001 v1.1 | TST-001 v1.1 / CP-01 |
Commits realizados / PR pendiente | En implementación |

## 7. Observaciones
Este documento constituye el Elemento de Configuración TRA-001.
La versión 1.0 representa la trazabilidad correspondiente a la configuración inicial de SoftEdu establecida en BL-001.
La versión 1.1 registra el impacto y las relaciones generadas por la solicitud de cambio CR-001 - Agregar teléfono al
estudiante.

CR-001 fue revisada y aprobada por erikaucp,  mediante el PR #2 y PR#3 e integrada en main.

Esta actualización documental corrige las referencias que permanecían como pendientes y registra el estado final del
cambio.

La creación de la línea base 1.1 será realizada posteriormente por el owner.

RF-03 y RF-04 conservan trazabilidad parcial porque sus funcionalidades todavía no están implementadas.

Una vez que el cambio sea revisado y aprobado mediante Pull Request, esta matriz deberá actualizar el estado de CR-001,
registrar la referencia al Pull Request y reflejar la nueva línea base que se establezca.
