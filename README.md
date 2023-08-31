
# Advanced permissions

In this repo, you will find a few example roles that you can use with [Beefree SDK](https://beefree.io/bee-plugin/ "https://beefree.io/bee-plugin/"), an embeddable drag-and-drop content editor. For an overview of this feature, please refer to our [dedicated page](https://docs.beefree.io/advanced-permissions/ "https://docs.beefree.io/advanced-permissions/") in our documentation website.

## Role templates

The following templates demonstrate various roles but can be customized or extended to address specific use cases. For a detailed explanation of the fields and the JSON structure, head to [our docs](https://docs.beefree.io/advanced-permissions/ "https://docs.beefree.io/advanced-permissions/").

### The copywriter

This template allows the end-user to edit text and images but disables all other behaviors and settings. This skill-based role is for people in an organization who only need to touch copy for editing or translation purposes. Copy the contents of `copywriter.json` into the `advancedPermissions` variable of your bee config to enable the following behaviors:

-   Hide any action that doesn’t involve working on a copy of an email or page.
    
-   Limit style options for the text itself by
    
    -   locking/hiding the side tab
        
    -   Hiding specific settings in the text toolbar
        

### The file manager

This template limits how users upload and manage images and files inside the builder to select pre-approved images and files uploaded by “admin” users. Copy the contents of `fileManager.json` into the `advancedPermissions` variable of your bee config to enable the following behaviors:

-   Disabling drag-and-drop of images onto the stage;
    
-   Limit actions in the file picker (either the builders or your [custom file picker)](https://docs.beefree.io/custom-file-picker/ "https://docs.beefree.io/custom-file-picker/") by disabling actions like upload, import, and create a folder.
