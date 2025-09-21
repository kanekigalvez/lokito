# Vice City 3D Prototipo

Un prototipo de juego 3D en Three.js inspirado en GTA Vice City, con una ciudad de 500x500 unidades, 500 NPCs caminando (estilo GTA V), edificios neón, palmeras, y tiendas interactivas. Incluye un sistema de dinero y colisiones.

## Características
- **Mapa**: Terreno de 500x500 con calles, 50 edificios, 30 palmeras.
- **NPCs**: 500 NPCs animados (modelo CesiumMan) moviéndose aleatoriamente.
- **Interacciones**: Acércate a NPCs (compra snacks por 5 monedas) o tiendas (gana 20 monedas) con la tecla E.
- **Controles**: WASD para mover, Espacio para saltar, E para interactuar.
- **Optimizaciones**: Fondos oscuros, iluminación ajustada, modelos fallback si GLTF falla.

## Cómo ejecutar
1. **GitHub Pages**:
   - Accede a la URL: `https://tu-usuario.github.io/tu-repositorio/`.
   - Ejemplo: (reemplaza con tu URL tras configurar GitHub Pages).
2. **Localmente**:
   - Clona el repositorio: `git clone https://github.com/tu-usuario/tu-repositorio.git`.
   - Navega a la carpeta: `cd tu-repositorio`.
   - Inicia un servidor local: `python -m http.server 8000`.
   - Abre `http://localhost:8000/index.html` en Chrome/Firefox.
3. **Rendimiento**:
   - Si laggea, edita `index.html` y cambia `const maxNpcs = 500;` a `100`.

## Requisitos
- Navegador moderno (Chrome/Firefox recomendado).
- Conexión a internet para cargar Three.js y CesiumMan.glb.
- Hardware decente para 500 NPCs (reduce si es necesario).

## Solución de problemas
- **Pantalla blanca**: Verifica la consola (F12). Asegúrate de usar un servidor local o GitHub Pages para evitar CORS.
- **Errores de carga**: Comprueba las URLs de Three.js y el modelo GLTF.
- **Lag**: Reduce `maxNpcs` a 100 o menos en el código.

## Créditos
- Modelo NPC: CesiumMan.glb (KhronosGroup).
- Inspirado en GTA V (peatones del video: https://www.youtube.com/watch?v=lSzX-mc_3JA).