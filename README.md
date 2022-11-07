# printClass

## About the project ##
Mendix Javascript action that sends one (the first) or all html elements on the screen that have a given identifier class to the print dialogue. From here, the user can decide to send the result to the printer or save the content as a pdf.

The main advantage is that the Javascript action also allows printing elements that are currently not supported by the Document templates (e.g., anyChart elements) 

## Typical usage scenario ##
When sending page content to the printer, one often only wants to print certain elements on the screen. For example, there may be a print button on the screen that does not need printing itself. In that case, you can use this Javascript action. Only those elements on the screen that have a identifier class added, will be sent to the printer.

## Configuration ##
* Add an identifier class to the element(s) that need printing
* Create a Nanoflow action that calls the JS_PRintClass Javascript action
* Set `Class name` tot he identifier class
* Set `Prints all occurances` to `true` when all elements with the identifier class need to be sent to the printer or `false` if only the first element with the identifier class needs to be sent to the printer.

## Sample project ##
https://printclass-sandbox.mxapps.io/

## Contributing ##
* Create feature branch from `develop`
* Create changes
* Create a pull request

## License
Apache v2.0

## Contact
marco.bouwkamp@mendix.com
