# Ourita

Ourita es un conversor de divisas en una sola página HTML con estética pixel retro futurista, dark mode y acentos neón pastel. Está planteado como un mini objeto digital centrado en pantalla: compacto, cute y directo.

## Qué incluye

- Conversión automática al cambiar moneda o cantidad
- Botón `swap` para invertir origen y destino
- Pantalla destacada para el cambio actual
- Diseño responsive tipo mini consola
- Footer discreto con enlaces personales
- Detalles visuales pixelados: rejilla, corazones, brillos y microanimaciones

## Stack

- HTML
- CSS
- JavaScript vanilla

## Fuente de datos

Ourita usa el endpoint abierto de ExchangeRate-API:

- [https://open.er-api.com/v6/latest/USD](https://open.er-api.com/v6/latest/USD)

La app consulta dinámicamente la moneda base seleccionada y muestra la última actualización disponible que devuelve la API.

## Archivo principal

- [conversor_divisas_cute.html](C:\Users\isasa\OneDrive\Desktop\jornaling\conversor_divisas_cute.html)

## Cómo abrirlo

1. Abre `conversor_divisas_cute.html` en el navegador.
2. Elige moneda de origen y destino.
3. Escribe la cantidad.
4. La conversión se actualiza automáticamente.

## Decisiones de diseño

- El nombre visible de cada moneda aparece en el desplegable para que la lectura sea más natural.
- El código ISO se mantiene como etiqueta secundaria bajo cada selector para no perder precisión.
- El botón de intercambio se sitúa entre ambas monedas para que su función se entienda visualmente de un vistazo.
- El resultado tiene más glow y jerarquía que el resto para atraer la mirada.

## Si quieres personalizarlo

- Cambia colores globales en `:root`
- Ajusta la estética del dispositivo en `.device`
- Modifica la pantalla principal en `.screen`
- Cambia enlaces del footer en el bloque `.micro-footer`
- Edita las monedas en el objeto `currencies`

## Posibles siguientes mejoras

- Búsqueda dentro de los desplegables
- Persistencia de última combinación usada
- Historial corto de conversiones
- Selector de idioma
- Modo “compact” todavía más minimal
