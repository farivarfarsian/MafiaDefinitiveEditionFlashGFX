# Adding New Buttons To The Main Menu:
So now go to this line for example:

![Screenshot (272)](https://user-images.githubusercontent.com/63361129/142378722-5e9b5976-df51-47b0-a283-d3784577dded.png)

And try to change the P-Code 
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

When you done coding it, save the gfx file, pack the SDS File and see the results by running the game.
