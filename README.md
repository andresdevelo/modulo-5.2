# 🥡 Proyecto: Menú Aleatorio de Especiales – China Bistro

## 📋 Resumen

En esta tarea, vamos a mejorar la experiencia del usuario en la aplicación web del restaurante **David Chu's China Bistro**. La página principal cuenta con tres mosaicos interactivos: **Menú**, **Especiales** y **Mapa**. Anteriormente, al hacer clic en el mosaico de **Especiales**, siempre se mostraban los artículos de una categoría fija del menú.

### 🧠 ¿Qué haremos?

Modificaremos el comportamiento de **Especiales** para que, al hacer clic, se redirija a una **categoría aleatoria** del menú (como "Lunch", "Dinner", "Sushi", etc.), mostrando sus artículos correspondientes.

---

## 🔧 Cambios realizados

### 1. 📁 Modificación del snippet `home-snippet.html`

Se editó el fragmento HTML para que contenga un marcador `{{randomCategoryShortName}}` en la función de llamada al hacer clic sobre el mosaico "Specials":

```html
<a href="#" onclick="$dc.loadMenuItems({{randomCategoryShortName}});">
