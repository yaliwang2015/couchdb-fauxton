# Extensions

Extensions allow Fauxton views to be have extra functionality.

A module registers an extension by

    FauxtonAPI.registerExtension('extensionName', myObjectToRegister);

Any other module wanting to use that extension can then get 
all objects registered for an extension by:

    var extensions = FauxtonAPI.getExtensions('extensionName');
    // extensions will always be an array

The module can then use those extensions to extend its functionality.
