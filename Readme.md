Ya no estoy trabajando en el Término final en este momento. El puerto está completo y es "utilizable" pero no se ha implementado la emulación vt102 completa.

La reescritura
El Término final original dependía de Clutter y Mx que ya no son viables. El objetivo principal de esta bifurcación fue portar Final Term a GTK + 3.0, lo que le dio un gran impulso al rendimiento. Esta portabilidad está completamente completa. Se ha implementado alguna emulación adicional de vt102, pero aún queda un largo camino por recorrer.

Acerca del término final
Final Term es una nueva generación de emuladores de terminal.

Va más allá de la mera emulación y comprende lo que sucede dentro del shell que aloja. Esto le permite ofrecer funciones que ningún otro terminal puede ofrecer, que incluyen:

Menús de texto semántico
Finalización inteligente de comandos
Controles de terminal GUI
Instalación
El término final está escrito en Vala y construido sobre GTK + 3 . Requiere los archivos de desarrollo para los siguientes paquetes de software:

Caramba
GTK + 3
keybinder-3.0
libnotify Opcional , para soporte de notificaciones de escritorio
libunity Opcional , para la integración del lanzador de Unity (barras de progreso)
Además, requiere intltool para la extracción de cadenas de localización.

Para instalar las dependencias en ubuntu, ejecute los siguientes comandos:

# Build tools
sudo apt-get install intltool cmake make valac

# Required
sudo apt-get install libgtk-3-dev libkeybinder-3.0-dev libgee-0.8-dev libjson-glib-dev

#Optional
sudo apt-get install libunity-dev libnotify-dev
Para instalar Final Term, ejecute estos comandos de shell:

clon de git https://github.com/RedHatter/finalterm-reborn.git
 cd finalterm-reborn /
compilación de mkdir
construcción de cd /
cmake ..
hacer
sudo make install
Si desea instalar en un directorio personalizado, su XDG_DATA_DIRSvariable de entorno debe apuntar al prefijo que contiene el archivo glib-2.0/schemas/gschemas.compiled.

Expresiones de gratitud
Final Term debe gran parte de su existencia a la genialidad de Vala y su documentación , Clutter y Mx , así como a la generosa decisión de los autores de esos proyectos de lanzar su increíble trabajo como software de código abierto.

Gran parte del conocimiento sobre la emulación de terminal necesario para construir Final Term se obtuvo de la especificación xterm y la Guía del usuario de VT100 , así como del estudio de emuladores de terminal existentes como st y Terminator .

Los esquemas de color de Final Term se generan utilizando el maravilloso Base16 Builder de Chris Kempson.

El icono de la aplicación de Final Term es una versión modificada del icono del terminal del tema del icono de Faenza de Matthieu James.

Licencia
Copyright © 2013–2014 Philipp Emanuel Weidmann ( pew@worldwidemann.com )
Copyright © 2015-2016 RedHatter ( timothy@idioticdev.com )

Final Term es software libre: puede redistribuirlo y / o modificarlo según los términos de la Licencia Pública General GNU publicada por la Free Software Foundation, ya sea la versión 3 de la Licencia o (a su elección) cualquier versión posterior.

Final Term se distribuye con la esperanza de que sea útil, pero SIN NINGUNA GARANTÍA; incluso sin la garantía implícita de COMERCIABILIDAD o APTITUD PARA UN PROPÓSITO PARTICULAR. Consulte la Licencia pública general de GNU para obtener más detalles.

Debería haber recibido una copia de la Licencia Pública General GNU junto con el Término Final. Si no es así, consulte http://www.gnu.org/licenses/ .
