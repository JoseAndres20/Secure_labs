# Secure_labs — 📚 Documentación de máquinas

> 📁 Repositorio **solo** para documentación paso a paso de máquinas/labs resueltas (HackTheBox, TryHackMe, DockerLabs, VMs propias, etc.).  
> ❗ Aquí **no** se suben VMs, ISOs ni binarios; solo `README.md` (walkthrough) y capturas/evidencias en `img/`.

---

<!-- Badges (reemplaza los links si quieres) -->
[![Estado](https://img.shields.io/badge/estado-documentaci%C3%B3n-brightgreen)](#)
[![Contenido educativo](https://img.shields.io/badge/licencia-CC--BY--NC--SA--4.0-blue)](LICENSE)
[![Aviso legal](https://img.shields.io/badge/uso-educativo-orange)](#)

---

## 🎯 Propósito
Centralizar **writeups reproducibles** organizados por **plataforma → máquina → documentación**. Cada máquina incluye un `README.md` con pasos reproducibles (reconocimiento → explotación → post-explotación), referencia a evidencias en `img/` y recomendaciones de mitigación.

---
```
## 📂 Estructura recomendada (visual)
Secure_labs/
├─ machines/
│ ├─ HackTheBox/
│ │ ├─ machine-sicario/
│ │ │ ├─ README.md # walkthrough (comandos, outputs, notas)
│ │ │ └─ img/ # capturas: YYYY-MM-DD_HH-MM_descripcion.png
│ │ └─ machine-omega/
│ │ ├─ README.md
│ │ └─ img/
│ ├─ TryHackMe/
│ │ └─ machine-basico/
│ │ ├─ README.md
│ │ └─ img/
│ ├─ DockerLabs/
│ │ └─ machine-webapp/
│ │ ├─ README.md
│ │ └─ img/
│ └─ OtraPlataforma/
│ └─ machine-ejemplo/
│ ├─ README.md
│ └─ img/
├─ templates/
│ └─ machine-template.md
├─ .gitignore
├─ LICENSE
└─ README.md ← (este archivo)

```

---

## ✍️ Convenciones mínimas por máquina
- Carpeta: `machine-XXX-nombre-corto/`  
- Dentro:
  - `README.md` → Documentación completa.
  - `img/` → Capturas y diagramas.
- `README.md` debe incluir:
  1. **Título**, **Autor / Alias**, **Fecha**  
  2. **Resumen ejecutivo** (2–3 líneas)  
  3. **Entorno / Plataforma** (Origen: HTB / THM / DockerLab / VM)  
  4. **Pasos reproducibles** (comandos exactos; incluye outputs clave)  
  5. **Evidencias** (referencias a `img/filename.png`)  
  6. **Conclusiones y mitigaciones**  
- Nombres de imagen: `YYYY-MM-DD_HH-MM_descripcion.png` (ej.: `2025-10-30_14-23_nmap.png`).

---

## ✅ Checklist rápido para PRs
- [ ] `README.md` de la máquina usa plantilla y es reproducible.  
- [ ] `img/` contiene al menos 1 captura referenciada.  
- [ ] No hay archivos grandes de VM, ISOs o binarios.  
- [ ] No se subieron credenciales ni `.env` con secretos.  
- [ ] `metadata.yml` (opcional) con `author`, `date`, `platform`, `tags`.

---

## ⚖️ Legal / Ética
> Material para uso educativo en entornos controlados.  
> No intentes explotar sistemas sin autorización. El repositorio no facilita acceso a máquinas reales; solo documenta resoluciones.

---

## 🧩 Plantilla rápida (usar para cada `README.md`)
```markdown
# machine-XXX — <Título>

**Autor:** <Alias>  
**Fecha:** YYYY-MM-DD  
**Plataforma origen:** <HackTheBox / TryHackMe / DockerLabs / VM>  
**Estado:** Resuelta / Documentada

## Resumen ejecutivo
(2–3 líneas)

## Entorno / IP de pruebas
- Tipo: VM / Docker
- IP: 10.10.10.5 (ej.)

## Reconocimiento
```bash
nmap -sC -sV -oN nmap-basic.txt 10.10.10.5
# resultados relevantes...
Explotación — pasos reproducibles
Paso 1 — comando — evidencia: img/xxx.png

Paso 2 — comando — evidencia: img/yyy.png

Post-explotación / Escalada
Usuario obtenido: <user>

LPE: pasos y evidencias

Conclusiones y mitigaciones
Recomendaciones técnicas

---
*Hecho con ❤️ — mantén el repo limpio y enfocado en documentación.*  
