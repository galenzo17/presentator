---
title: "Un Repo Para Gobernarlos a Todos"
theme: seriph
favicon: "https://cdn.jsdelivr.net/gh/slidevjs/slidev@main/packages/docs/public/favicon.png"
download: true
layout: cover
background: "https://source.unsplash.com/random/1920x1080?tech"
transition: fade
---

# Consolidación Máxima de Repositorios

<small>(...y buena vibra de paso)</small>

---

## ¿Por qué Unirlos?

transition: fade

- **Menos** caos
- **Más** orden
- **Más** risas en el daily
- ¡Y menos quebraderos de cabeza!

<v-click>

> "Tres repos entran a un bar…  
> Se unifican en uno y ¡la fiesta sigue!"

</v-click>

---

## La Idea

transition: fade

**Objetivo Principal:**  
Un solo lugar para:

1. **Autenticación**
2. **Jobs/Reportes**
3. **Endpoints API**

<v-click>

> “Todos los problemas en un solo repositorio… ¡para solucionarlos más fácil!”

</v-click>

---

## Nueva Estructura de Carpetas

transition: fade

```bash
my-awesome-api/
├─ auth/          # Todo lo de Dashboard
├─ jobs/          # Lo de Workflows
├─ reports/       # Reportes centralizados
├─ database/      # Acceso unificado
├─ api/           # Endpoints (¡bye repos dispersos!)
└─ ...
```

<v-click>

    Minimalismo + Organización
    = ¡Código feliz!

</v-click>

---

## Estrategia en Fases

transition: fade

    Fase 1: Traer login y autenticación
    Fase 2: Migrar reportes y tareas programadas
    Fase 3: Unificar base de datos
    Fase 4: Ordenar endpoints y hacerlo bonito

<v-click>

    ¡Todos a bordo con tiempo, sin romper nada en producción!

</v-click>

---

Ejemplo Rápido

transition: fade

// Pequeño snippet de autenticación (auth/login.js)
try {
  // Lógica de autenticación
  const user = await authenticate(req.body)
  res.json({ success: true, user })
} catch (error) {
  res.status(401).json({ success: false, error: error.message })
}

<v-click>

    En un solo repo: ¡Autenticación clarita y sin doble código!

</v-click>

---

Beneficios a Ojo de Buen Cubero

transition: fade

    Mantenimiento más sencillo
    Más velocidad en desarrollos
    Monitoreo central
    Cero despliegues confusos

<v-click>

    Menos estrés, más tiempo para café ☕

</v-click>

---

Cosas a Evitar

transition: fade

    Reinventar la rueda (no refactores locos)
    Cambiar todo de golpe (no se rompan corazoncitos en producción)
    Olvidar las pruebas (nadie quiere bugs)

<v-click>

    “Con calma y con tests, nada sale mal.”

</v-click>
¿Listos para la Unión?

transition: fade class: text-center
¡Un repo para gobernarlos a todos!
<div v-click> <img src="https://media.giphy.com/media/l4FGpP4lxGGgK5CBW/giphy.gif" alt="Celebración" width="300"/> </div>
¡Gracias!

transition: fade layout: center class: text-center

¡A unificar y a triunfar!

---

---
title: "Demo: Magic Move en Slidev"
magic: true
transition: fade
---

# Paso 1

```js
// Versión Inicial
function greet() {
  console.log("¡Hola, mundo!");
}
```

```js
// Versión Actualizada
function greet(name) {
  console.log(`¡Hola, ${name}!`);
}
```
