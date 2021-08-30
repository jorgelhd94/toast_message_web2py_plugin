# Web2py Toast Message Plugin

This is a Web2py plugin for manage message in the view using the toast library. For install this plugin is necessary use the plugin manager of the web2py framework.

## Requirements

1. Use Boostrap 4 library
2. Include web2py_ajax.html file in the layout

## Function plugin_toastr_message_config()

`plugin_toastr_message_config('type_message', 'message_text', ajax=False)`

### 
+ ty

## Usage
 
After installing the plugin in the web2py plugin manager it is necessary to add a few lines of code in the main layout.

1. Add the next code to view/layout.html (the main layout) into the body tag

+ `{{=plugin_toastr_message()}}`  
+ ``<div id="plugin-toastr-message">``  
+ ``</div>``

2. To launch the message, include the next code in a controller.

`plugin_toastr_message_config('success', 'All good', ajax=False)

Or

`plugin_toastr_message_config('error', 'Oops!! An error has occurred!', ajax=False)

  
