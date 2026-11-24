# lavappdora.com

Web estática de Lavappdora: landing y páginas legales. HTML y CSS a mano, sin build, sin JavaScript y sin recursos de terceros (ni fuentes, ni analítica, ni cookies).

| Archivo | Qué es |
|---|---|
| `index.html` | Landing |
| `privacidad.html` | Política de privacidad (incluye cookies) |
| `aviso-legal.html` | Aviso legal (LSSI-CE, art. 10) |
| `condiciones.html` | Condiciones de uso de la app |
| `404.html` | Página de error de GitHub Pages |
| `css/estilos.css` | Estilos de todo el sitio |
| `img/` | Icono y capturas de la app |
| `CNAME` | Dominio propio para GitHub Pages |

## Datos legales

Titular y correo de contacto están en `privacidad.html`, `aviso-legal.html` y `condiciones.html`. Si cambian, hay que actualizarlos en las tres páginas.

## Ver en local

```bash
python3 -m http.server 8765 --directory .
```

y abre http://localhost:8765.

## Publicar en GitHub Pages

1. Crea el repositorio en GitHub y súbelo (rama `main`).
2. En *Settings → Pages*: *Source* = *Deploy from a branch*, rama `main`, carpeta `/ (root)`.
3. El archivo `CNAME` ya pide el dominio `lavappdora.com`. En el proveedor del dominio crea:
   - Cuatro registros `A` para `lavappdora.com` hacia `185.199.108.153`, `185.199.109.153`, `185.199.110.153` y `185.199.111.153`.
   - Un `CNAME` para `www` hacia `<usuario>.github.io`.
4. Cuando GitHub verifique el dominio, marca *Enforce HTTPS*.

## Datos de la tira de precios

La tira de la landing usa el PVPC real del 24/11/2026 descargado de REData (Red Eléctrica). Si se cambia, hay que mantener la cita de la fuente bajo el gráfico.
