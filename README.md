# Diario de motivación

Aplicación web (React + Vite) para guiar al alumnado en un diario reflexivo por pasos, con resumen final imprimible en A4.

## Funcionalidades

- Flujo guiado: introducción + 4 pasos + resumen.
- Captura de datos del alumno: nombre, curso, asignatura y SdA.
- Intereses y estado emocional con visualización gráfica.
- Lluvia de ideas con posicionamiento en ejes X/Y.
- Resumen final imprimible en una sola página A4.
- Personalización por URL: `dep`, `sda`, `curso`, `asignatura`.

## Requisitos

- Node.js 20+ (recomendado)
- npm

## Desarrollo local

1. Instalar dependencias:

```bash
npm install
```

2. Ejecutar en modo desarrollo:

```bash
npm run dev
```

3. Abrir en navegador:

- `http://localhost:3000`

## Build de producción

```bash
npm run build
```

Este comando:

- genera la app en `dist/`
- copia este `README.md` a `dist/README.md`

## Vista previa del build

```bash
npm run preview
```

## Parámetros de URL

Puedes precargar datos de contexto y matrícula usando query params:

- `dep`: departamento
- `sda`: situación de aprendizaje
- `curso`: curso del alumno
- `asignatura`: nombre de asignatura

Parámetros alternativos soportados por compatibilidad:

- `grade` (equivalente a `curso`)
- `subject` (equivalente a `asignatura`)

### Ejemplo completo

```text
http://localhost:3000/?dep=Departamento%20de%20Tecnolog%C3%ADa%20e%20Inform%C3%A1tica&sda=Lenguajes%20de%20programaci%C3%B3n&curso=2%C2%BAESO&asignatura=Tecnolog%C3%ADa%20y%20Digitalizaci%C3%B3n
```

### Formatos de curso aceptados

La app normaliza automáticamente formatos habituales:

- `1ESO`, `1ºESO`
- `2ESO`, `2ºESO`
- `3ESO`, `3ºESO`
- `4ESO`, `4ºESO`
- `1BACH`, `1ºBACH`, `1ºBACHILLERATO`
- `2BACH`, `2ºBACH`, `2ºBACHILLERATO`

## Scripts disponibles

- `npm run dev`: desarrollo local
- `npm run build`: build de producción
- `npm run preview`: servir build localmente
- `npm run clean`: borrar `dist`
- `npm run lint`: comprobación de TypeScript sin emitir
