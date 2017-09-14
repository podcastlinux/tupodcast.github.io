Muy buenas!!!  
Como siempre, muchas ideas en la cabeza y con ganas de aportar.

Vamos a hacer un alojamiento para **publicar un podcast mediante archive.org y Github Pages + Jekyll.**    
Gracias a Ugeek y otros muchos, he conocido esta manera asequible de crear un blog a tu podcast y que te ofrezca el feed.

Toda la info la he extraído de:  
<https://github.com/barryclark/jekyll-now>  
<https://github.com/ugeek/ugeek.github.io/>  
<https://devexperto.com/blog-gratis-github-jekyll/>

Vamos paso a paso: Puede parecer un poco lío al principio, pero en 30 minutos puedes tener tu blog activo.

1. **Crea tu cuenta github** con el nombre de tu podcast <https://github.com/> Ej:frentealmicro  

2. **Realiza un fork** de este repositorio: <https://github.com/podcastlinux/tupodcast.github.io>  
Ve a esta página y haz clic en Fork

3. **Modifica y configura tu Github Pages** con tu info y logo para que funcione como un blog.  
**Cambia el nombre del repositorio** en Settings a tuusuario.github.io Ej:frentealmicro.github.io  
**Edita _config.yml** (clic en el icono del lápiz) con tu nombre del podcast, descripción, avatar (logo), redes sociales y no te olvides todo lo referente al feed del podcast en la parte # Podcast Feed Settings 
No te olvides de grabar los cambios en el botón Commit changes.  
Sube tu logo a la carpeta images. Por ejemplo: logo.png. Te aconsejo 3000x3000 px. Lo puedes crear con [Inkscape](https://inkscape.org/es/)  
Una vez ya hayas hecho esto, deberías poder acceder a tu blog desde cualquier navegador: tuusuario.github.io  
A veces no es automático y tarda un poco. Si se demora mucho, vuelve a editar

Es muy interesante que actives [Disqus](https://disqus.com/) para tener comentarios de los oyentes en el blog.   
Para no perderte,revisa este archivo de [ejemplo](https://github.com/podcastlinux/podcastlinux.github.io/blob/master/_config.yml)  
También puedes **editar about.md** para poner todos tus métodos de contacto y algo de info sobre tu podcast.

4. **Crea una cuenta en <https://archive.org>.**

5. **Aloja tus archivos de audio y extrae la url** de ellos.  
Añade con upload el archivo de audio (arriba con el símbolo fecla hacia arriba) y rellena los campos.  
Una vez esté, entra en ese audio [(Ejemplo)](https://archive.org/details/PL28Aniversario) y pincha en [VBR mp3](https://ia800605.us.archive.org/26/items/PL28Aniversario/PL-28-Aniversario.mp3) o si lo prefieres en formato [Ogg Vorbis](https://ia800605.us.archive.org/26/items/PL28Aniversario/PL-28-Aniversario.ogg)  
Copia el link de esa url

6. Aprende a **realizar los posts** para que salgan como episodios de tu podcast.
En tu repositorio accede a la carpeta _post.  
Dentro de ella tendrás un archivo de ejemplo en formato .txt  
Copia y modifica su nombre y añade dentro las notas del programa.  
El archivo debe ser año-mes-día-nombre-del-episodio.md Ejemplo: 2017-09-15-promo.md    
Al principio tienes una zona para definir el post (datos de ejemplo). Es muy importante poner en __categories:podcast__ para que cargue esta entrada como episodio del feed.    
~~~
_layout: post  
title: "Promo Frente al Micrófono"  
date: 2017-09-15  
categories: podcast  
image: images/logo.png  
podcast_link: https://ia800605.us.archive.org/26/items/PromoFrentealmicrófono/FAM-00-promo.mp3  
tags: [audio, promo, Frente al Micrófono]  
comments: true_  
~~~
Puedes añadir imágenes, links, tablas, vídeos... cualquier cosa.  
Para conocer más Markdown, el lenguaje que utiliza para la edición de texto, mira este [post](https://markdown.es/sintaxis-markdown/)  
Te dejo un [ejemplo](https://github.com/uGeek/ugeek.github.io/edit/master/_posts/podcast/2017-09-04-076.-Un-servidor-en-mi-casa.md) y cómo se ve en el [blog](https://ugeek.github.io/076.-Un-servidor-en-mi-casa/)

7. **Revisa** que **el feed** esté bien.
Una vez ya tengas tu primer episodio, verifica que todo haya ido bien.  
Probemos a ver si tu feed funciona. Tu feed es: tuusuario.github.io/feed
Puedes utilizar un podcatcher para ver si carga correctamente. En Android te recomiendo [Antennapod](https://play.google.com/store/apps/details?id=de.danoeh.antennapod&hl=es)  
También pudes probar esta página:<http://castfeedvalidator.com/>  


Cualquier duda me puedes encontrar en:  
<li>Twitter: <a href="https://twitter.com/podcastlinux">@podcastlinux</a></li>
<li>Telegram: <a href="https://t.me/juanfebles">@juanfebles</a></li>
<li>Correo: <a href="mailto:podcastlinux@gmail.com">podcastlinux@gmail.com</a></li>
<li>Blog: <a href="https://podcastlinux.github.io">podcastlinux.github.io</a></li>
