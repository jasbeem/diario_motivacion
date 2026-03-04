# Diario de Aprendizaje

Aplicación web (React + Vite) para guiar al alumnado en un diario reflexivo por pasos, con resumen final imprimible en A4.

## Funcionalidades

- Flujo guiado: introducción + 4 pasos + resumen.
- Captura de datos de alumno/a, curso, asignatura y SdA.
- Intereses y estado emocional con visualización gráfica.
- Lluvia de ideas con posicionamiento en ejes X/Y.
- Resumen final preparado para impresión/PDF en una sola página A4.
- Personalización por URL con parámetros `dep` y `sda`.

## Requisitos

- Node.js 20+ (recomendado).
- npm.

## Desarrollo

1. Instalar dependencias:

```bash
npm install
```

2. Iniciar en local:

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

- genera los archivos compilados en `dist/`
- copia este `README.md` a `dist/README.md`

## Vista previa del build

```bash
npm run preview
```

## Parámetros de URL

Puedes precargar departamento y situación de aprendizaje:

```text
http://localhost:3000/?dep=Departamento%20de%20Tecnolog%C3%ADa%20e%20Inform%C3%A1tica&sda=Lenguajes%20de%20programaci%C3%B3n
```

## Scripts disponibles

- `npm run dev`: desarrollo local.
- `npm run build`: build de producción.
- `npm run preview`: servir build localmente.
- `npm run clean`: borrar `dist`.
- `npm run lint`: comprobación de TypeScript sin emitir.
