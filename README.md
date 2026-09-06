# Dulus Premium updates.

This repository is the public release channel for Dulus Premium desktop
artifacts. It contains release binaries and their SHA-256 sidecars only; the
Premium source code and customer data stay private.

<img width="1371" height="1207" alt="HRU8-zPaoAAunno" src="https://github.com/user-attachments/assets/0b3c88f8-40be-4507-8b2c-054c2de36c92" />


## Release contract

- Tags use `vX.Y.Z` (for example `v3.12.0`).
- Windows: `Dulus-X.Y.Z-windows-setup.exe`
- macOS Apple Silicon: `Dulus-X.Y.Z-macos-arm64.dmg`
- macOS Intel: `Dulus-X.Y.Z-macos-x86_64.dmg`
- Linux: `Dulus-X.Y.Z-linux.AppImage`
- Each installer should ship with a matching `<asset>.sha256` sidecar.

Premium checks this channel once at startup and then once every 24 hours while
the app is open. Updates are announced non-blockingly; the user opens the
GitHub release page and installs the signed artifact manually.

v6.0.6 > v6.0.7 Changelog:

I HAVENT FULLY DEBUG THE APP BUT THE PERFORMANCE WAS BASTLY INCREASED, I RATHER YOU FACING SOME BUGS THAT YOU RUNNING A SHITTY CODE ♥

My commits in the last 3 days for our private Dulus Build... this is my last time showing my creativity...

I will code it.

🚀 Dulus v6.0.6 ➡️ v6.0.7 Changelog 🚀

✨ Nuevas Features & Core • 👁️ Control de Pantalla Nativo: Agregadas las herramientas ScreenGround y ScreenClick para uso nativo de la computadora.

• ♾️ Lookback Auto-Recall: Nuevo sistema push-RAG que le da contexto virtualmente "infinito" a los modelos locales pequeños.

• 🔒 Modo Isolate: El toggle /isolate ahora bloquea todas las herramientas de escritura, edición y Bash para que no salgan de tu workspace.

• ⏳ Waits Inteligentes: Ahora la IA prefiere usar Reminder en lugar de Bash('sleep N') para esperar, evitando bloquear el chat.

🧠 Razonamiento y Memoria

• 💭 Streaming Real: El comando /thinking vuelve a ser el control principal para el razonamiento, ahora con verdadero streaming.

• 🛡️ Memoria Robusta: Timeout guard implementado para mempalace y protección para evitar que el archivo de memoria se encoja. El baseline de gold/soul ahora va directo al system prompt.

• 🗣️ Verbose Thinking: Restaurado para proveedores como LiteLLM, DeepSeek y Qwen.

🖥️ Interfaz y Experiencia (GUI)

• 📁 Mejoras en el Workspace: Panel de contexto con auto-apertura y subidas de hasta 25MB directamente al workspace.

• 🖱️ El menú de /load ahora es clickeable y se eliminó el molesto bug del ícono duplicado en el Dock.

• 🔤 ¡Adiós acentos rotos (mojibake)! Decodificación UTF-8 estricta para el SSE de Meta y ChatGPT.

• ❄️ Solucionado el problema del escritorio congelado al arrancar (seeding correcto de memoria a corto plazo).

🌐 Modelos y Proveedores

• 🦙 Soporte añadido para Meta AI Muse Spark (http://api.meta.ai/v1/responses). • ✖️ Nuevo alias de proveedor x ➡️ xai-oauth (para Grok-4.5).

• 🤖 Configuración predeterminada actualizada: ahora por defecto usa el modelo dulus/dulus-a-9b, permission_mode=auto y webdrive_embed=always.

• 🪪 Ahora enviamos la identidad de Dulus en los headers al comunicarnos con los LLMs.

🛠️ Infraestructura, DevOps & Fixes

• 🛑 Fail Fast: Eliminados los reintentos silenciosos.

Si un modelo falla, lo hace rápido para evitar que el agente "se congele de la nada".

• ☁️ Migración Cloud: El provisionador de entornos para clientes ha sido portado de Azure a OVH MKS.

• 📊 Arena de Benchmarks: Nueva arena para comparar modelos con un sistema de evaluación basado en evidencias.

• ⚙️ Protocolo de salida en JSON (--output json) y flujo de early-cut mejorado (welcome/doctor). 🔐 Seguridad & Agentes (Datadog-bits)

• Parcheados múltiples vectores críticos: mitigada la inyección de prompts en el bucle de herramientas del Army worker. • Fix de Path Traversal de tenants vía X-Tenant-ID. • Prevención de filtrado de datos (leaks) en el endpoint de búsqueda de memoria y en el marketplace. • Validación estricta del código autogenerado para plugins antes de escribir en el sistema.

⚡️ That's some homework for the industry!

Building binaries!
