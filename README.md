# DevOps Portfolio

Demostración del flujo Gitflow aplicado a scripts de administración Linux.

## Flujo de trabajo

| Rama | Propósito | Se crea desde | Merge hacia |
|------|----------|--------------|------------|
| main | Producción | — | — |
| develop | Integración continua | main | main (via release) |
| feature/* | Nuevas funcionalidades | develop | develop |
| release/* | Preparación de versión | develop | main + develop |
| hotfix/* | Correcciones urgentes | main | main + develop |

## Scripts incluidos

- scripts/sistema.sh
- scripts/verificar-permisos.sh
- scripts/fix-log-perms.sh

## Versiones

- v1.0 — Release inicial
- v1.1 — Hotfix de permisos
