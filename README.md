[README.md](https://github.com/user-attachments/files/32572820/README.md)
# Dashboard de Producción

Dashboard web estático listo para GitHub Pages.

## Archivos
- `index.html`: interfaz y lógica del dashboard.
- `data.json`: datos consumidos por el dashboard.

## Publicar en GitHub Pages
1. Crea un repositorio en GitHub.
2. Sube `index.html` y `data.json` a la raíz del repositorio.
3. Ve a **Settings > Pages**.
4. En **Build and deployment**, selecciona **Deploy from a branch**.
5. Selecciona la rama `main` y la carpeta `/ (root)`.
6. Guarda y espera a que GitHub publique el sitio.

## Probar localmente
No abras el HTML con doble clic. Desde esta carpeta ejecuta:

```bash
python -m http.server 8000
```

Después abre `http://localhost:8000`.

## Corrección aplicada
La función `visible()` ahora muestra por defecto los registros cuando el campo `Visible` o `Registro visible` no existe, y admite `1`, `true`, `si` y `sí` como valores visibles.
