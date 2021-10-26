# Mafia Definitive Edition Flash Language Documentation

## Get Started
For Editing Flash Files(.gfx) We use [JPEX Flash Decompiler](https://github.com/jindrapetrik/jpexs-decompiler/releases)
In Mafia Definitive Edition Main Flash Files are in ```MAINGAMEFOLDER/sds_retail/gui```

For Unpacking SDSs Files You Should use [Mafia Toolkit](https://github.com/Greavesy1899/MafiaToolkit/releases/tag/2.21)

### Adding New Buttons To The Main Menu:
```actionscript
getproperty QName(PrivateNamespace("pages:main_menu_page_main"),"ButtonTypes")
findpropstrict QName(PackageNamespace("components"),"ButtonData") 
getlex QName(PrivateNamespace("pages:main_menu_page_main"),"CARCYCLOPEDIA") 
pushstring "YOURSTRINGNAME"
constructprop QName(PackageNamespace("components"),"ButtonData"), 2
callpropvoid QName(Namespace("http://adobe.com/AS3/2006/builtin"),"push"), 1
debugline 197
getlocal0
```
#### Let Break this Down Line By Line:

1-Calling Add Button Types Function
```actionscript
getproperty QName(PrivateNamespace("pages:main_menu_page_main"),"ButtonTypes")
```
2-Creating New Button
```actionscript
findpropstrict QName(PackageNamespace("components"),"ButtonData")
```
3-Calling The Function (First Argument)
```actionscript
getlex QName(PrivateNamespace("pages:main_menu_page_main"),"CARCYCLOPEDIA")
```
4-Push Your Custom String with pushstring(Second Argument)  
```actionscript
pushstring "YOURSTRINGNAME"
```
5-Specifies The Button Type/Data And Pushes Them
```actionscript
constructprop QName(PackageNamespace("components"),"ButtonData"), 2
callpropvoid QName(Namespace("http://adobe.com/AS3/2006/builtin"),"push"), 1
```
6-Debugging Line Which Program use For Debugging But it doesn't matter 
```actionscript
debugline 197
```
7-Ending The Function
```actionscript
getlocal0
```
