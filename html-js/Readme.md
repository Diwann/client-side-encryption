client-side-encryption
==========
Sample code for client-side encryption

JavaScript version 0_1_6
---

The 0_1_6 version of the JavaScript client-side encryption library fixes an issue in older Firefox where the native random number generator throws a not implemented exception.

JavaScript version 0_1_5
---

The 0_1_5 version of the JavaScript client-side encryption library upgrades the random number generator and the JSBN implementation.
 

JavaScript version 0_1_4
---
 The 0_1_4 version of the JavaScript client-side encryption offers a LuhnCheck and default validations on other fields.

 All properties are configurable through the options object:

 * ```options.enableValidations // default: true```
 
   Enable basic field validation (default is true)

   The submit button will be disabled when fields proof to be invalid. The form submission will be prevented as well.

    ```javascript
    options.enableValidations = true;
    ```
 * ```options.submitButtonAlwaysEnabled // default: false```
 
   Always have the submit button enabled, even in case of validation errors.
 
   ```javascript
   options.submitButtonAlwaysEnabled = false;
   ```
 * ```options.numberIgnoreNonNumeric // default: true```
 
 The payment handling ignores non-numeric characters for the card field.
 
 By default non-numeric characters will also be ignored while validating
 the card number field. This can be disabled for UX reasons.

 ```javascript
  options.numberIgnoreNonNumeric = true;
 ```

 Patches
 
 * 0_1_4p1
 
     Remove unnecessary ```document.title``` assignment.