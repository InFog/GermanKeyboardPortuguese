# German keyboard with Portuguese special chars

The `de` file contains the keyboard map for the "German Legacy" layout, that
was recently removed from some GNU/Linux distros.

In order to reenable it you should copy the `de` file to `/usr/share/X11/xkb/symbols/`.

Here is the command, in case you need it:

`# cp de /usr/share/X11/xkb/symbols/`

Then run the keyboard configuration helper:

`dpkg-reconfigure keyboard-configuration`

And select "German Legacy" on the layout option.

If the option "German Legacy" does not show up in the configuration then you can
force it on XFCE itself. To do so you should edit the file
`.config/xfce4/xfconf/xfce-perchannel-xml/keyboard-layout.xml` to add the "legacy"
variation. The file will lok like this:

```xml
<?xml version="1.0" encoding="UTF-8"?>

<channel name="keyboard-layout" version="1.0">
  <property name="Default" type="empty">
    <property name="XkbDisable" type="bool" value="false"/>
    <property name="XkbLayout" type="string" value="de"/>
    <property name="XkbVariant" type="string" value="legacy"/>
  </property>
</channel>
```

# Teclado alemão com caracteres especiais em Português

O arquivo `de` contém o mapa de teclado para o layout "German Legacy", que foi
recentemente removido de algumas distribuições GNU/Linux.

Para poder habilitar este layout copie o arquivo `de` para `/usr/share/X11/xkb/symbols/`.

Aqui está o comando, no caso de você precisar dele:

`# cp de /usr/share/X11/xkb/symbols/`

Então utilize o comando para configurar o layout do teclado:

`dpkg-reconfigure keyboard-configuration`

E selecione "German Legacy" na opção de layout.

Se a opção "German Legacy" não aparecer na configuração então você pode forçar
a opção direto no XFCE. Para fazer isso edite o arquivo
`.config/xfce4/xfconf/xfce-perchannel-xml/keyboard-layout.xml` para adicionar
a variante "legacy". O arquivo deve ficar parecido com isso:

```xml
<?xml version="1.0" encoding="UTF-8"?>

<channel name="keyboard-layout" version="1.0">
  <property name="Default" type="empty">
    <property name="XkbDisable" type="bool" value="false"/>
    <property name="XkbLayout" type="string" value="de"/>
    <property name="XkbVariant" type="string" value="legacy"/>
  </property>
</channel>
```
