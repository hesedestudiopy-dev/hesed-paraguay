# HESED Paraguay - Sitio web estático

Sitio web HTML/CSS/JS listo para publicar en GitHub Pages, OCI, Nginx, Apache o cualquier hosting estático.

## Opción recomendada gratis: GitHub Pages con URL limpia

1. Crear una organización o usuario en GitHub llamado `hesedpy`.
2. Crear un repositorio público llamado exactamente:

```bash
hesedpy.github.io
```

3. Subir estos archivos al repositorio.
4. Activar GitHub Pages desde:

```text
Settings > Pages > Deploy from a branch > main > /root > Save
```

5. La web quedará disponible en:

```text
https://hesedpy.github.io/
```

## Opción con tu usuario actual de GitHub

Crear un repositorio separado, por ejemplo:

```bash
hesed-paraguay
```

La URL será:

```text
https://TU_USUARIO.github.io/hesed-paraguay/
```

En este caso actualizar en `index.html`, `robots.txt` y `sitemap.xml` la URL base.

## Comandos para subir

```bash
git init
git add .
git commit -m "Sitio inicial HESED Paraguay"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/hesed-paraguay.git
git push -u origin main
```

## Importante para no solapar con Nexatec

- No usar el repositorio `nexatec-erp`.
- No usar la carpeta `/opt/nexatec` en el servidor.
- No reutilizar el mismo dominio/subdominio que Nexatec.
- Para GitHub Pages, no se usa la IP de OCI, por lo tanto no afecta al sistema Nexatec.
