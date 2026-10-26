# Vision Rover Challenge — UDLA

Laboratorio web de robótica virtual para estudiantes de enseñanza media.

## Funcionalidades
- Navegación del Rover mediante teclado, controles en pantalla y tarjetas monocromáticas.
- Simulador 2D con tres dificultades, obstáculos, cronómetro, colisiones y puntuación.
- Editor de instrucciones con AVANZAR, RETROCEDER, GIRAR_DERECHA, GIRAR_IZQUIERDA, ESPERAR, REPETIR/FIN y PARAR.
- Visión computacional local con cámara del navegador y marcadores binarios B/N.
- Tarjetas imprimibles en [tarjetas.html](tarjetas.html).

## Publicación
1. Abrir **Settings > Pages** en GitHub.
2. Configurar **Build and deployment > Source: GitHub Actions**.
3. Esperar que termine el flujo **Publish Vision Rover** en Actions.
4. Visitar https://droscarl.github.io/vision-rover-challenge/.

## Ejecución local
Desde esta carpeta: `python -m http.server 8000` y abrir `http://localhost:8000`.

## Uso
Iniciar desafío, navegar y llegar al sector META. El reconocimiento requiere permiso para cámara y origen seguro (HTTPS o localhost). Se recomienda Chrome o Edge actualizado.

## Estado y limitaciones
Prototipo educativo: la clasificación de tarjetas es geométrica y **no** emplea una red neuronal. El algoritmo de visión requiere validación con webcams y tarjetas impresas en el entorno real. No se almacena ni transmite el vídeo de la cámara. Los programas son interpretados localmente, sin ejecutar JavaScript introducido por estudiantes. La programación y los controles visuales deben calibrarse para diferentes cámaras e iluminación.
