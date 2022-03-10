# URLS-de-Movistar-TV-Manifest-DASH-

<H2>Esto es solo un estudio o descubrimiento , en ningun momento se pretende disfrutar del contenido ilegalmente y ni mucho menos lucrarse de ello, entenderlo de esta manera, gracias</H2>


El otro dia estaba viendo una web de TV legal con canales nacionales y tenia un iframe escondido de un canal de Movistar+. Me dio curiosidad y por lo tanto vi su codigo fuente y se trataba de un manifest con DRM con la sorpresa que ponia telefonica en el principio de la dirección. Me informe un poco en Google y ya hace unos años, un chico llamado Aitor descubrio las URLS de la vieja plataforma Movistar TV Go.

Dejo el enlace por aqui

https://www.linkedin.com/pulse/c%C3%B3mo-descubr%C3%AD-las-urls-de-los-canales-movistar-tv-go-mag%C3%A1n-garc%C3%ADa/?originalSubdomain=es

En ese año la sintasis de la URL era de esta manera

http://B31317.cdn.telefonica.com/31317/ANTENA3_SUB.m3u8 

Lo que venia a ser que 
http://BXXXXX.cdn.telefonica.com/ XXXXXX/ NOMBRE-CANAL-ACORTADO_SUB.m3u8

El prinicipio de la B era el identificador del canal seguido otra vez este mismo pero sin la b y el canal de TV abreviado con un guion y SUB.

El pobre Aitor fue buena gente en su momento y aviso a la misma compañia del fallo pero claro estamos en España y no le dieron ni una mierda.
Hasta hoy he descubierto que la nueva sintasis ( hasta dia de hoy 08/03/22) es de la siguiente manera. 

https://b43987-p8-h83-aejx8pov.1.cdn.telefonica.com/_43987/dash/mligacampeones.isml/manifest.mpd





Este es un ejemplo de MLCampeones. EL prinicipio de la B es exactamente igual a la vieja URL , pero ya luego lo han complicado un poco. En este caso sigue de un p8-h83 pero ya les digo que en cada canal es totalmente diferente y por lo tanto cambia, por ejemplo en otro canal seria p5-h99. Ya luego sigue igual que antes con el ID del canal , seguido de la tegnologia DASH e ISML ( que viene a ser el formato de stream) junto a la abreviatura del canal y terminando con manifest.mpd. Vamos que estan codificiados a diferencia de hace unos años que el M3U8 se reproducia directamente teniendo conexión a Internet.

La cosa es que si tienes la clave del stream se reproduciria directamente como pasa en esta pagina 
![image](https://user-images.githubusercontent.com/17550010/157147582-ce4410f1-ef85-47dc-8c6e-03931a7e58b8.png)





No entiendo mucho de como reproducir manifest tan facil como lo es como el M3U8, en eso ya me pierdo. Se que hay herramientas para estos temas como FFMPEG y Youtube-DL


____________________________________________________________________________________________________________________________________________________
Fin de la Charleta dejo las URLS que he pillado :D


M+ liga
https://b43955-p8-hb6-aemx8pov.1.cdn.telefonica.com/_43955/dash/mlaliga.isml/manifest.mpd
M+ Campeones
https://b43987-p8-h83-aejx8pov.1.cdn.telefonica.com/_43987/dash/mligacampeones.isml/manifest.mpd
M+ Campeones 1
https://b44016-p8-h35-aemh8pov.1.cdn.telefonica.com/_44016/dash/01campeones.isml/manifest.mpd
M+ Campeones 3
https://b44018-p8-hb3-aelx8pov.1.cdn.telefonica.com/_44018/dash/03campeones.isml/manifest.mpd
M+ Campeones 4
https://b44019-p8-h89-aejh8pov.1.cdn.telefonica.com/_44019/dash/04campeones.isml/manifest.mpd
M+ Campeones 5
https://b44020-p8-hec-aeoh8pov.1.cdn.telefonica.com/_44020/dash/05campeonesor.isml/manifest.mpd
M+ Campeones 6
https://b44021-p8-hcb-aelx8pov.1.cdn.telefonica.com/_44021/dash/06campeonesor.isml/manifest.mpd





Por ultimo , recordar que el chaval que habia mencionando antes que lo habia descubierto desde el primer promento habia desarollado un script en Python para buscar Canales o urls mediante la sintaxis que le pongas. Les dejo el enlace para que le echeis un ojo :). 
https://gist.github.com/aitormagan/41c9b044e0511184bf63






