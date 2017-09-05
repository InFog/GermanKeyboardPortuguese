# German keyboard with Portuguese special chars

The `de` file contains the keyboard map for the "German Legacy" layout, that
was recently removed from some GNU/Linux distros.

In order to reenable it you should copy the `de` file to `/usr/share/X11/xkb/symbols/`.

Here is the command, in case you need it:

`# cp de /usr/share/X11/xkb/symbols/`

Then run the keyboard configuration helper:

`dpkg-reconfigure keyboard-configuration`

And select "German Legacy" on the layout option.

# Teclado alemão com caracteres especiais em Português

O arquivo `de` contém o mapa de teclado para o layout "German Legacy", que foi
recentemente removido de algumas distribuições GNU/Linux.

Para poder habilitar este layout copie o arquivo `de` para `/usr/share/X11/xkb/symbols/`.

Aqui está o comando, no caso de você precisar dele:

`# cp de /usr/share/X11/xkb/symbols/`

Então utilize o comando para configurar o layout do teclado:

`dpkg-reconfigure keyboard-configuration`

E selecione "German Legacy" na opção de layout.
