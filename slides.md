---
layout: center
background: https://cover.sli.dev
---

## El pitch del Agus 

![Danza divertida](https://media2.giphy.com/media/v1.Y2lkPTc5MGI3NjExNzhxc3BxNTNnZ21oNWQxM3VxMDB6NWRmZTQ3Y25wMGVmY2o0emV4aiZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/l0He4fJxPCbfqv7Xi/giphy.webp)


---
layout: center
---

## Migracion autenticación usuarios dashboard a la Api
````md magic-move
```js {*}{lines:true,startLine:5}
Problema

Actualmente, la lógica de autenticación está dividida entre la API y el Dashboard, 
lo que genera:
-    Duplicación de lógica y puntos de falla.
-    Mayor complejidad en el mantenimiento o actualización del flujo de autenticación.
-    Dificultad para garantizar la seguridad y consistencia de los tokens en todos los servicios.
-    Retos en la supervisión y resolución de problemas de acceso de usuarios.

Esta capa dispersa de autenticación complica la escalabilidad y el mantenimiento adecuado del sistema.
```
```js {*}{lines:true,startLine:5}
Solución

Unificar la funcionalidad de autenticación en la API principal, 
dejando el Dashboard como un cliente que consume 
esta autenticación centralizada.
```
```js {*}{lines:true,startLine:5}
Arquitectura Unificada

    Implementar un módulo centralizado de autenticación y autorización en la API.
    Redirigir todos los endpoints de autenticación del Dashboard hacia la API.
    Mantener una estructura modular que permita agregar o modificar flujos de
     autenticación de forma independiente.
```
```js {*}{lines:true,startLine:5}
Beneficios Esperados

    Reducción en la complejidad del mantenimiento.
    Mayor seguridad al unificar la gestión de tokens y credenciales.
    Implementación simplificada de nuevos flujos de autenticación.
    Monitoreo más detallado de eventos de login y logout.
    Ciclos de desarrollo más rápidos para nuevos requerimientos de autenticación.
```
```js {*}{lines:true,startLine:5}
Fuera de Alcance

    Reescribir funcionalidades no relacionadas con la autenticación.
    Cambiar contratos de la API fuera del flujo de autenticación.
    Modificar esquemas de base de datos más allá de lo estrictamente 
    necesario para la autenticación.
```
````

---
title: Amazing slide title
layout: center
---

Migracion 
<span v-mark="{ at: 2, color: '#234', type: 'circle' , strokeWidth:8, padding:9 }">
autenticación
</span>
 usuarios dashboard a la Api
