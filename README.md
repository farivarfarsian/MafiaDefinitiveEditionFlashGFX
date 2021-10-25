# Mafia Definitive Edition Flash Language Documentation

## Adding New Buttons To The Main Menu:
```actionscript
getproperty QName(PrivateNamespace("pages:main_menu_page_main"),"ButtonTypes")
findpropstrict QName(PackageNamespace("components"),"ButtonData")
getlex QName(PrivateNamespace("pages:main_menu_page_main"),"CARCYCLOPEDIA")
pushstring "$carcyclopedia"
constructprop QName(PackageNamespace("components"),"ButtonData"), 2
callpropvoid QName(Namespace("http://adobe.com/AS3/2006/builtin"),"push"), 1
debugline 197
getlocal0
```
