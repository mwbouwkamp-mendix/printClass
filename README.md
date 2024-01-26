# printClass

## About the project ##
Mendix module that sends one (the first) or all html elements on the screen that have a given identifier class to the print dialogue or saves these html elements to a pdf file.

The main advantage is that the Javascript action also allows printing elements that are currently not supported by the Document templates (e.g., anyChart elements).

## Typical usage scenario ##
When sending page content to the printer, one often only wants to print certain elements on the screen. For example, there may be a print button on the screen that does not need printing itself. In that case, you can use this Javascript action. Only those elements on the screen that have a identifier class added, will be sent to the printer.

Instead of sending targeted page content to the printer, the module also allows creating a corresponding pdf.

## Configuration ##
* Add an identifier class to the element(s) that need printing
* Create a Nanoflow action that calls the JS_PrintClass_Printer / JS_PrintClass_PDF Javascript action
* Set `Class name` tot he identifier class
* Set `Prints all occurances` to `true` when all elements with the identifier class need to be sent to the printer or `false` if only the first element with the identifier class needs to be sent to the printer.

## Sample project ##
https://printclass-sandbox.mxapps.io/

## License
Apache v2.0

## Contact
marco.bouwkamp@mendix.com
