La siguiente página esta basada en una interfaz parecida a una tienda electronica de videojuegos;
Para esta práctica se realizó la página enfocada en la empresa de Nintendo.

Aquí se encuentran las 15 páginas locales que son las siguientes:
*index.html - Página Home (principal).
*contact.html - Página de contacto.
*shop.html - Página de venta de los videojuegos.
*categories-1.html - Página donde se encuentran la categoría de juegos de peleas. 
*categories-2.html - Página donde se encuentran la categoría de juegos de rol por turno.
*categories-3.html - Página donde se encuentran la categoría de juegos multijugador. 
*categories-4.html - Página donde se encuentran la categoría de juegos de aventura.
*categories-5.html - Página donde se encuentran la categoría de juegos de terror. 
*product-details.html - Página donde se encuentra la descripción del producto Nintendo Switch. 
*product-details-1.html - Página donde se encuentra la descripción del producto The Binding of Isaac: Repentance.  
*product-details-2.html - Página donde se encuentra la descripción del producto Super Smash Bros Ultimate.
*product-details-3.html - Página donde se encuentra la descripción del producto Luigi's Mansion 3. 
*product-details-4.html - Página donde se encuentra la descripción del producto Xenoblade Chronicles: Definitve Edition.
*product-details-5.html - Página donde se encuentra la descripción del producto OMORI.
*product-details-6.html - Página donde se encuentra la descripción del producto Pokémon Scarlet.

Las páginas remotas, son 5 y son las siguientes:
*Página oficial de Nintendo sobre el producto Fortnite.
*Página oficial de Nintendo sobre el producto Metroid Prime Remastered.
*Página oficial de Nintendo sobre el producto Animal Crossing.
*Página oficial de Nintendo sobre el producto Minecraft.
*Página oficial de registro de Nintendo.

Para montar la página en el servidor, se instaló previamente Apache en Ubuntu y después se ejecutó el siguiente comando en la
terminal para copiar el la carpeta que contiene todas las páginas en el servidor.
sudo cp -r /home/nombreUsuario/carpetaPagina /var/www/html/

Y para cambiar el nombre de la página cuando es vista en el navegador primero se utilizó el siguiente comando:
sudo chmod 777 hosts

Acto seguido se abre el siguiente archivo con cualquiera de los comandos.
nano hosts 
ó
gedit hosts

Se agrega la siguiente línea en el archivo
direccionip nombre 
por ejemplo:
172.16.1.137 proyecto

Y por último se reinicia el servicio con el siguiente comando.
sudo service apache2 restart

Luego se visita la página con el siguiente link:
http://nombre/ruta/de/la/pagina