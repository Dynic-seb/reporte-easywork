# Reporte Easywork — Meta Ads

Reporte ejecutivo de la campaña de Meta Ads de Easywork, generado y mantenido por dynic.

🔗 **Ver el reporte en vivo:** https://dync-seb.github.io/Reporte-Easywork/
*(la URL exacta la confirma GitHub al activar Pages — puede diferir levemente, ver paso a paso)*

## Qué es esto

Un reporte HTML autocontenido (sin backend, sin build, sin dependencias que instalar) con el desempeño de la campaña de captación de leads de Easywork: leads generados, presupuesto invertido, costo por lead (CPL), CTR, campañas activas, mejores anuncios, mejor zona geográfica, evolución diaria y comparativa semana a semana.

Se actualiza **una vez por semana** con datos exportados de Meta Ads Manager.

## Cómo actualizar el reporte

1. Exportar el CSV actualizado desde Meta Ads Manager (nivel anuncio × región × día).
2. Recalcular las métricas y regenerar `index.html` con los datos nuevos (mismo formato y estructura).
3. Subir el archivo actualizado:
   - **Por la web de GitHub:** entrar al repo → *Add file* → *Upload files* → arrastrar el nuevo `index.html` → escribir un mensaje de commit (ej. "Actualización semana del 05/10") → *Commit changes*.
   - **Por terminal**, si preferís git:
     ```bash
     git add index.html
     git commit -m "Actualización semana del DD/MM"
     git push
     ```
4. GitHub Pages redeploya solo, en 1–2 minutos. El link no cambia entre actualizaciones.

## Estructura del repo

- `index.html` — el reporte completo (HTML + CSS + Chart.js vía CDN). GitHub Pages lo sirve automáticamente como página principal porque se llama `index.html`.
- `README.md` — este archivo.

## Stack

HTML estático + [Chart.js](https://www.chartjs.org/) (vía CDN) + Google Fonts (DM Serif Display, DM Sans, Poppins). Sin build, sin backend, sin dependencias que instalar.

## Nota sobre privacidad

Este repo es **público** (requisito de GitHub Pages en el plan gratuito). El reporte contiene datos reales de leads y gasto de Easywork — cualquiera con el link puede verlo. Si en algún momento se pasa a un plan de GitHub pago, se puede pasar el repo a privado sin perder Pages.
