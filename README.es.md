# 六韬（LT）

[中文](./README.md) · [English](./README.en.md) · [日本語](./README.ja.md) · [한국어](./README.ko.md) · [Français](./README.fr.md)

Six Strategies es un protocolo de colaboración de ingeniería de software para Codex. Organiza tareas complejas de desarrollo, reparación, refactorización y mantenimiento a largo plazo en un flujo trazable y verificable.

## Capacidades principales

- `R-`: registra requisitos observables y criterios de aceptación.
- `A-`: registra arquitectura, límites, invariantes y decisiones clave.
- `F-`: divide el trabajo en lotes de implementación con propiedad clara de archivos.
- `T-`: fija pruebas, comandos y evidencias revisables.
- Aplica puertas específicas a la arquitectura base, contratos públicos, permisos, migraciones, IPC, plugins, compilación y publicación.

## Flujo de trabajo

```text
Fijar objetivos → evaluar impacto → elegir arquitectura mínima
    → implementar → verificar → actualizar memoria → auditar → registrar cambios
```

SOL se ocupa de la arquitectura crítica aún no fijada, los contratos públicos, la implementación crítica indivisible y la auditoría final. Luna se ocupa de la recopilación de hechos y de la implementación, verificación y documentación con decisiones ya fijadas y alcance limitado.

## Instalación

[Descarga el ZIP desde Release](https://github.com/Taian1738/six-strategies/releases/download/v2026.08.21/ltskill-20260821-142646.zip), extráelo en `<CODEX_HOME>/skills/ltskill/` y conserva la estructura de directorios. Después puedes invocarlo explícitamente con `$ltskill`.

Versión del protocolo: `LT-2026-08-21.11`


