# BWAPI Uso del API The Brood War [(UAlbertaBot)](https://github.com/davechurchill/ualbertabot)

## Especificaciones del Equipo

* Intel(R) Core(TM) i7-4700MQ CPU @ 2.40GHz 64 bits
* 8GB RAM
* Windows-10

## Instalación
### Prerequisitos
  * Visual Studio 2013
  * StarCraft: Brood War(1.16.1)
  * BWAPI
  * [BWTA 2.2](https://bitbucket.org/auriarte/bwta2/downloads)
  
### Variables Locales
 Añadir las siguientes variables en My Computer > Click Properties > Click Advanced System Settings > Click Environment Variables > Click New...
 * `BWAPI_DIR` - BWAPI 4.1.2 installation root directory
* `BWTA_DIR` - BWTA 2.2 installation root directory
### ¿Cómo compilar?
1. Abrir `UAlbertaBot / VisualStudio / UAlbertaBot.sln` en Visual Studio 2013
2. Editar la función `onStart ()` en `UAlbertaBotModule.cpp` para que la llamada a` parseConfigFile () `indique dónde se encuentra el archivo de configuración de UAlbertaBot en la máquina. 
2. Seleccionar el modo `Release`
3. Construir el proyecto UAlbertaBot (todos los proyectos serán construidos)
4. Despues compilado el .dll irá al directorio `UAlbertaBot / bin`
### ¿Cómo ejecutar?
1. Verificar que Starcraft: Broodwar sea la versión 1.16.1
2. Instalar BWAPI
3. Verifficar de que `Chaoslauncher.exe` y` Starcraft.exe` estén configurados para ejecutarse como administrador.( Propiedades> Compatibilidad> Ejecutar como administrador)
4. Ejecutar `Chaoslauncher.exe` (viene con BWAPI)
5. Modificar la configuración BWAPI de Chaoslauncher para que apunte al compilado `UAlbertaBot.dll`
  * En Chaoslauncher, haga clic en la opción `BWAPI 4.1.2 Injector [RELEASE]` y asegúrese de que esté marcada
  * Haga clic en el botón `Config` cerca de la parte inferior y editar el parámetro `ai` para apuntar a su` ruta / a / UAlbertaBot.dll` y guardar
6. Editar el [archivo de configuración de UAlbertaBot] (UAlbertaBot-Configuration-File)
7. Ejecutar StarCraft usando Chaoslauncher
8. Para probar el bot, inicie un juego usando Single Player> Expansion> Play Custom, seleccionar cualquier mapa multijugador estándar y usar la configuración` Melee` para comenzar.


## Capturas de la ejecución
<img src="/images/sc1.png" alt="Screenshot1"/>
<img src="/images/sc2.png" alt="Screenshot1"/>
<img src="/images/sc3.png" alt="Screenshot1"/>
<img src="/images/sc4.png" alt="Screenshot1"/>



