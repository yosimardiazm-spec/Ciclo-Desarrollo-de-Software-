# 🔥 Configuración de Firebase - DevCycle Quest

Este proyecto puede funcionar de dos formas:

## 🚀 Opción 1: Red Local (Funciona ya)
- **Profesor y estudiantes en la misma red/dispositivo**
- **Sin necesidad de Firebase**
- El juego usa `localStorage` y `BroadcastChannel`

## 🌐 Opción 2: Cualquier Red (Firebase)
Para permitir que profesor y estudiantes accedan desde **redes diferentes**:

### Paso 1: Crear proyecto Firebase
1. Ve a [https://firebase.google.com](https://firebase.google.com)
2. Click en "Ir a la consola"
3. Click en "Crear un proyecto"
4. Nombre: `devcycle-quest` (o el que quieras)
5. Aceptar términos y crear

### Paso 2: Agregar app web
1. En el proyecto → Click el ícono web `</>` 
2. Nombre de la app: `DevCycle Quest`
3. Click "Registrar app"
4. Copiar la configuración que aparece

### Paso 3: Habilitar Realtime Database
1. En el menú izquierdo → "Realtime Database"
2. Click "Crear una base de datos"
3. Ubicación: Elegir la más cercana
4. Modo de seguridad: **Prueba (público)**
5. Click "Habilitar"

### Paso 4: Configurar en el código
Abre `index.html` y busca:

```javascript
const FIREBASE_CONFIG = {
  apiKey: "AIzaSyDemoKeyChangeMe",
  authDomain: "tuproyecto.firebaseapp.com",
  projectId: "tuproyecto",
  databaseURL: "https://tuproyecto.firebaseio.com",
  storageBucket: "tuproyecto.appspot.com",
};
```

Reemplaza con tus credenciales de Firebase (del paso 2)

### Paso 5: Deploy a GitHub Pages
```bash
git add .
git commit -m "Firebase configured"
git push -u origin main
```

## ✅ Listo!
Ya puedes:
- Profesor abre desde cualquier dispositivo/red
- Estudiantes abren desde otro dispositivo/red
- Ingresan el código y ¡juegan!

## 🔒 Considersaciones de Seguridad
- En producción, cambia el modo de seguridad de "Prueba" a reglas más restrictivas
- Agrega autenticación si es necesario
- Limpia bases de datos antiguas periódicamente

## ❌ Si no configuras Firebase
- **Funciona igual en red local**
- Los estudiantes solo pueden acceder desde la misma red/dispositivo
- Perfecto para aula presencial

---

¿Preguntas? Revisa la consola del navegador (F12) para debug logs.
