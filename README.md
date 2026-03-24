# 🎮 DevCycle Quest — Ciclo de Desarrollo de Software

> Juego educativo multijugador para estudiantes de **Ingeniería Informática (8vo Semestre)**.  
> Temática: NovaTech S.A.S. debe entregar un sistema hospitalario. Tú eres el Tech Lead.

🔗 **Jugar en vivo:** [https://TU-USUARIO.github.io/devcycle-quest](https://TU-USUARIO.github.io/devcycle-quest)

---

## 🚀 Cómo publicar en GitHub Pages (5 minutos)

### Opción A — Interfaz web de GitHub (sin instalar nada)

1. Ve a [github.com](https://github.com) e inicia sesión
2. Clic en **"New repository"**
3. Nombre: `devcycle-quest` · Marca **"Public"** · Clic **"Create repository"**
4. En la página del repo, clic **"uploading an existing file"**
5. Arrastra los dos archivos: `index.html` y `README.md`
6. Clic **"Commit changes"**
7. Ve a **Settings → Pages → Source → Deploy from branch → main → / (root)**
8. Guarda. En ~1 minuto estará en: `https://TU-USUARIO.github.io/devcycle-quest`

### Opción B — Git desde terminal

```bash
git clone https://github.com/TU-USUARIO/devcycle-quest.git
cd devcycle-quest
# Copia index.html y README.md aquí
git add .
git commit -m "feat: DevCycle Quest multijugador"
git push origin main
```

Luego activa GitHub Pages en **Settings → Pages**.

---

## 🎯 Cómo usar en clase

### El Profesor (pantalla grande / proyector)
1. Abre el link → **"Soy el Profesor"**
2. Elige la dificultad → **CREAR SALA**
3. Aparece un código de 4 letras → proyéctalo
4. Espera que los estudiantes se conecten → **INICIAR JUEGO**

### Los Estudiantes (celular o PC)
1. Abren el mismo link → **"Soy Estudiante"**
2. Ingresan el código del proyector
3. Escriben su nombre y eligen avatar
4. ¡A jugar!

> ⚠️ **Importante:** La comunicación entre pantallas usa `BroadcastChannel`, que funciona entre **pestañas del mismo navegador**. Para dispositivos físicos distintos, todos deben abrir el mismo link en la **misma red**.  
> La solución más robusta para clase real: usar el link de GitHub Pages (todos abren la misma URL).

---

## 🔥 Modos de Dificultad

| Modo | ⏱ Timer | ❤️ Vidas | 💡 Pistas | ☠️ Trampas |
|------|---------|---------|----------|-----------|
| 🟢 Easy | 45s | ×5 | ✅ | — |
| 🔵 Normal | 30s | ×3 | ❌ | — |
| 🟠 Hard | 20s | ×2 | ❌ | — |
| 🔴 Very Hard | 15s | ×1 | ❌ | — |
| ☠️ Immortal Dev | 10s | ×1 | ❌ | Una opción extra que parece correcta pero es una trampa conceptual |

---

## 📚 Fases del SDLC cubiertas

1. 🗺️ **Planeación** — Project Charter, alcance, riesgos
2. 📋 **Requisitos** — RF vs RNF, SRS (IEEE 830), validación
3. 🎨 **Diseño** — Arquitectura de microservicios, persistencia políglota
4. 💻 **Desarrollo** — Scrum, Continuous Integration, trunk-based development
5. 🧪 **Pruebas** — Pirámide de testing, QA en software crítico
6. 🚀 **Despliegue** — Blue-Green Deployment, zero downtime
7. 🔧 **Mantenimiento** — Observabilidad (O11y), tipos de mantenimiento

---

## 🛠️ Tecnología

- **100% HTML/CSS/JS** — sin frameworks, sin dependencias, sin servidor
- **BroadcastChannel API** para comunicación entre pestañas
- **localStorage** para sincronización de estado de sala
- **Google Fonts** — Orbitron + Share Tech Mono + Rajdhani

---

## 📄 Licencia

MIT — libre para uso educativo. Desarrollado para Ingeniería Informática.
