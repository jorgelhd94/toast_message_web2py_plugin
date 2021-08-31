# Web2py Toast Message Plugin

This is a Web2py plugin for manage message in the view using the toast library. For install this plugin is necessary use the plugin manager of the web2py framework.

## Requirements

1. Use Boostrap 4 library in the layout
2. Include web2py_ajax.html file in the layout

## Function plugin_toastr_message_config()

`plugin_toastr_message_config('type_message', 'message_text', ajax=False)`

### Function arguments
* __type_message(string)__: Define the message css style. Can be:  

   + __success__: Show a success message  
   
   + __error__: Show an error message   

* __message_text(string)__: Define the message text.  
* __ajax(bool)__: Used when working with web2py ajax components. Allows the message to be displayed asynchronously:
    + **Important**: In case of using the messages in an asynchronous controller and using the response.js variable, it is necessary to call the __plugin_toastr_message_config()__ method after the last use of the response.js variable.

## Usage
 
After installing the plugin in the web2py plugin manager it is necessary to add a few lines of code in the main layout.

1. Add the next code to view/layout.html (the main layout) into the body tag:

+ `{{=plugin_toastr_message()}}`  
+ ``<div id="plugin-toastr-message">``  
+ ``</div>``

2. To launch the message, include the next code in a controller.

`plugin_toastr_message_config('success', 'All good', ajax=False)` 

![ok](https://user-images.githubusercontent.com/53158723/131509546-b31cbbed-4121-4b12-b01a-74d515a7b471.PNG)

Or

`plugin_toastr_message_config('error', 'Oops!! An error has occurred!', ajax=False)`

![error](https://user-images.githubusercontent.com/53158723/131508897-2c1ef4c3-59f8-4df0-9c8c-5abfd67a8074.PNG)


## Contributors

Many thanks to Ronald William Pérez Sánchez for his help.

  
