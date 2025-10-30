# Secure_labs — Documentación de máquinas

Repositorio dedicado **únicamente** a la documentación de máquinas/labs resueltas (HackTheBox, TryHackMe, DockerLabs, VMs propias, etc.).  
Aquí **no** se suben imágenes de disco ni binarios peligrosos: solo documentación (README/writeups) y capturas/evidencias en `img/`.

---

## Propósito
Centralizar writeups reproducibles y organizados por plataforma y por máquina: reconocimiento, explotación, post-explotación, evidencias y mitigaciones.

---
```
## Estructura recomendada
Secure_labs/
├─ machines/
│ ├─ HackTheBox/
│ │ ├─ machine-sicario/ # carpeta de la máquina
│ │ │ ├─ README.md # documentación paso a paso (walkthrough)
│ │ │ └─ img/ # capturas, diagramas, logs (nombres con timestamp)
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
└─ README.md
```


---

## Convenciones mínimas para cada `README.md` de máquina
- **Título**, **Autor / Alias** y **Fecha**.  
- **Resumen ejecutivo** (2–3 líneas).  
- **Pasos reproducibles** (comandos exactos y outputs relevantes).  
- **Evidencias**: referencias a imágenes en `img/` (usar nombres `YYYY-MM-DD_HH-MM_descripcion.png`).  
- **Conclusiones y mitigaciones**.  

---

## Reglas rápidas
- Cada máquina = 1 carpeta con `README.md` + `img/`.  
- No subir VMs, ISOs, contenedores o exploits compilados sin revisión.  
- No subir credenciales reales ni datos personales.  
- Añadir `LICENSE` y `CONTRIBUTING.md` si el repo será colaborativo.

---

## Nota legal
Material educativo: usar solo en entornos controlados y con permiso. No atacar sistemas fuera de laboratorios autorizados.

---

¿Quieres que genere ahora un `machine-template.md` (listo para copiar en `templates/`) con los apartados prellenables?  
