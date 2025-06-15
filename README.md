# OTCV8 Decrypt & Decompile Tool

Esta herramienta permite **descifrar** y **descompilar** archivos del cliente [OTClient V8](https://github.com/edubart/otclient) que están protegidos por el sistema de encriptación y compilación por defecto.

---

## 🛠️ Requisitos

- `otcv8_decrypt.exe`
- `luajit-descompilador.exe`
- Carpeta `encriptado` (con los archivos `.otmod` o `.lua` encriptados del cliente)
- (Opcional) Carpeta `descifrado` (será creada automáticamente si no existe)

---

### 🔓 Paso 1: Descifrar archivos

1. Coloca todos los archivos dentro de la carpeta llamada `encrypted`.
2. Ejecuta `otcv8_decrypt.exe`.
3. Espera a que finalice el proceso.
4. Los archivos descifrados aparecerán en la carpeta `decrypted`.

---

### 🧠 Paso 2: Descompilar bytecode LuaJIT

Después de descifrar, notarás que muchos de los archivos `.lua` aún están compilados en **bytecode LuaJIT**. Para convertirlos en código legible:

1. Arrastra y suelta el archivo `.lua` (o una carpeta completa) sobre `luajit-descompilador.exe`.
2. El descompilador procesará cada archivo y generará los archivos `.lua` legibles.


