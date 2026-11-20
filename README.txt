# American Flow — Speaking Coach

## Cómo ejecutar
1. Descomprime `American-Flow-PWA.zip`.
2. Sirve la carpeta mediante HTTPS o `localhost` (no abras `index.html` con doble clic).
3. En Windows puedes usar VS Code Live Server, o ejecutar `python -m http.server 8000` dentro de la carpeta y abrir `http://localhost:8000`.
4. En Chrome/Edge concede permiso al micrófono. Usa el botón de instalar aplicación del navegador.

## Qué incluye
- Repetición guiada con voz sintética en inglés estadounidense (`en-US`).
- Cuenta regresiva de 3 segundos y detección de fin de voz por silencio aproximado.
- Comparación de la transcripción reconocida con la frase modelo, sugerencias y repeticiones.
- Conversación guiada con 12 preguntas, respuestas modelo y sugerencias.
- Biblioteca con frases de los dos documentos, búsqueda y filtro.
- XP, racha, frases dominadas y estadísticas guardadas en `localStorage`.
- Manifiesto PWA, icono y service worker con caché del núcleo.

## Límites importantes
- La evaluación de pronunciación usa comparación de texto de Web Speech Recognition; NO es una puntuación fonética acústica como la de un motor especializado. No puede medir con fiabilidad la calidad de /θ/, /ð/, vocales, ritmo o entonación.
- La compatibilidad de `SpeechRecognition` varía por navegador y puede usar servicios remotos del navegador. El modo de voz no está garantizado offline. La voz disponible depende de las voces instaladas en el sistema.
- La conversación actual es guiada y basada en preguntas/reglas locales; no es un agente generativo de IA en tiempo real. Para una conversación libre con corrección fonética avanzada se requiere integrar un backend/API de voz, con clave protegida en servidor.
- Las transcripciones fonéticas de los documentos se conservan como material orientativo. Algunas formas son muy informales, regionales o dependientes del contexto; no todas deben usarse en entornos profesionales.


MEJORA PLUS DE AUDIO:
- Tres velocidades seleccionables: Natural 1.0x, Lenta 0.72x y Muy lenta 0.48x.
- Las tres velocidades mantienen la misma voz en-US y la misma frase.
- Puedes elegir entre las voces English (United States) disponibles en tu navegador/sistema.
- La calidad y naturalidad dependen de las voces instaladas en Windows/macOS/Android y del navegador; no se descarga una voz humana propietaria.
