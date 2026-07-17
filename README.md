# Mi lectura bíblica

App web de una sola página para llevar el registro de tu lectura bíblica: marcás tu progreso y lo podés sincronizar entre dispositivos con un código.

## Qué hace

- Registra el progreso de lectura y lo guarda en el navegador (`localStorage`).
- Sincroniza entre dispositivos usando un código personal (backend en Supabase).
- Permite cargar lecturas previas, respaldar y restaurar los datos.

## Stack

- HTML + CSS + JavaScript vanilla, todo en `index.html`. No hay build.
- Supabase como backend de sincronización (tabla `lectura_biblica`).

## Desarrollo local

Al ser un archivo estático, abrí `index.html` en el navegador, o servilo con cualquier servidor estático:

```bash
python3 -m http.server 8000
# luego abrí http://localhost:8000
```

## Despliegue

Alojado en Vercel. Cada push a `main` despliega automáticamente (integración con GitHub).

## Estructura

```
index.html   # toda la app: markup, estilos y lógica
icon.png     # ícono
```
