# Description

 - https://github.com/wilas/veewee-boxarium/tree/master/definitions/SL6_ks
 - https://github.com/wilas/veewee-boxarium/

## TODO

 - wget/curl installer
 - docs and manuals
 - manifest
 - bash like options (also --definition/--config def_file.cfg option)

## Hand installation

```
    sudo cp convert_2_scancode.py /usr/local/bin/
    sudo chmod 755 /usr/local/bin/convert_2_scancode.py
    cp vbkick.sh /usr/local/bin/vbkick
    sudo chmod 755 /usr/local/bin/vbkick
```

## convert_2_scancode.py

Enter key-strokes into a VirtualBox guest programmatically from the host:
```
$ VBoxManage controlvm VM_NAME keyboardputscancode $(echo 'Hello VM' | convert_2_scancode.py)
```

Example output keyboard scancodes:
```
$ echo -en 'Hello VM' | convert_2_scancode.py
2a 23 a3 aa 12 92 26 a6 26 a6 18 98 39 b9 2a 2f af aa 2a 32 b2 aa
```

## Bibliography

 - ! http://www.virtualbox.org/manual/ch08.html
 - ! http://www.jedi.be/blog/2009/11/17/controlling-virtual-machines-with-an-API/

