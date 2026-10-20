# La Despensa del Oso - Catálogo

## Cómo subir a GitHub Pages
1. Crea un repositorio y sube `index.html` y la carpeta `img/`.
2. Settings > Pages > Branch `main` > carpeta `/ (root)` > Save.

## Fotos de productos
Guarda cada foto en `img/` con el número de su producto (`01.jpg`, `02.jpg`...). También acepta `.png`. Si falta una foto, se muestra un ícono. Para combos usa `combo-1.jpg`, `combo-2.jpg`...

| Archivo | Producto |
|---|---|
| 01.jpg | Hamburguesa de carne - 390 g |
| 02.jpg | Milanesa - 400 g |
| 03.jpg | Hamburguesa de pollo - 400 g |
| 04.jpg | Nuggets - 500 g |
| 05.jpg | Albóndigas - 500 g |
| 06.jpg | Salchichas veganas clásicas - 500 g |
| 07.jpg | Salchichas veganas con finas hierbas - 500 g |
| 08.jpg | Chorizo vegano - 350 g |
| 09.jpg | Nuggets - 300 g |
| 10.jpg | Albóndigas - 300 g |
| 11.jpg | Carne de arvejas tipo nuggets - Bolsa 500 g |
| 12.jpg | Carne de arvejas tipo molida - Bolsa 500 g |
| 13.jpg | Carne de arvejas tipo nuggets - Bolsa 250 g |
| 14.jpg | Carne de arvejas tipo nuggets - Caja 100 g |
| 15.jpg | Carne de soya y gluten tipo bistec - Bolsa 500 g |
| 16.jpg | Gluten de trigo - Bolsa 500 g |
| 17.jpg | Soya tipo filete pollo - Bolsa 500 g |
| 18.jpg | Soya tipo filete res - Bolsa 500 g |
| 19.jpg | Soya pollo trozos - Bolsa 500 g |
| 20.jpg | Soya res trozos - Bolsa 500 g |
| 21.jpg | Soya pollo molido - Bolsa 500 g |
| 22.jpg | Soya res molida - Bolsa 500 g |
| 23.jpg | Soya pollo tiras - Bolsa 500 g |
| 24.jpg | Soya res tiras - Bolsa 500 g |
| 25.jpg | Soya tipo filete pollo - Caja 100 g |
| 26.jpg | Soya tipo filete res - Caja 100 g |
| 27.jpg | Soya pollo trozos - Caja 150 g |
| 28.jpg | Soya res trozos - Caja 150 g |
| 29.jpg | Soya pollo molido - Caja 150 g |
| 30.jpg | Soya res molida - Caja 150 g |
| 31.jpg | Soya pollo tiras - Caja 150 g |
| 32.jpg | Soya res tiras - Caja 150 g |
| 33.jpg | Fideos integrales de kiwicha - Caja 250 g |
| 34.jpg | Fideos integrales de espinaca - Caja 250 g |
| 35.jpg | Fideos integrales de pimiento - Caja 250 g |
| 36.jpg | Sal negra - 250 g |
| 37.jpg | Kañihua, harina seleccionada - Bolsa ziploc 200 g |
| 38.jpg | Harina de garbanzo - 250 g |
| 39.jpg | Agar agar |
| 40.jpg | Leche de almendras |
| 41.jpg | Leche de avena |
| 42.jpg | Alfajor argentino vegano |

## Combos
En `index.html` busca `const COMBOS` y agrega líneas como:
`["Combo Burger Día","2 hamburguesas + 1 chorizo",60],`

## Agregar productos nuevos
1. En `index.html`, dentro de `const PR=[`, agrega al final una línea: `["Nombre","Presentación",precio,""],` (el producto 39 será `39.jpg`, el 40 `40.jpg`...).
2. En `const C={`, agrega ese número a la lista de su categoría. Ejemplo: Suplementos `[39,40]`.

## Subcategorías
En `const C={`, una categoría con subcategorías se escribe así (cada subcategoría lleva su nombre y su lista de números):
`p:["Carnes vegetales","🥩",[["Nuggets",[4,9]],["Albóndigas",[5,10]]]],`
Una categoría simple lleva solo la lista de números: `o:["Otros","🧂",[36]],`
