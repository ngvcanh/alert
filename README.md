# Alert popup

* Using **Alert** object to create html popup.
* This Object need include JQuery.

## Create popup

````
Alert.popup(options);
````

* _options_: is an object of Javascript. The properties and methods of _options_:

**Name** | **Type** | **Mean**
--- | --- | ---
title _(string)_ | property | Title of popup, can use HTML
message _(string)_ | property | Content of popup, can use HTML
classes _(string)_ | property | Class color of popup (Value: _error_ (red), _success_ (green), _confirm_ (blue), _warning_ (orange))
iconClose _(boolean)_ | property | Display icon close popup (Default : ** _false_ **)
width _(string)_ | property | Width of popup, contains unit (**px** or __%__, Default : _300px_)
btn _(array)_ | property | List button below of popup, Each button is an object

With each button is an object, they are listed from right to left. Create button as follow:
````
{label : "OK", color : "red", isFocus : true, fn : Alert.close}
````

* **_label_** : Name of button will display, if it is not declared, the button will not be displayed.
* **_color_** : Color of button, Default is dark color (Value: red, green, blue, orange)
* **_isFocus_** : Focus to button after popup is appended page (Default: _false_)
* **_fn_** : function will call when click to button.

## Close popup

````
Alert.close()
````