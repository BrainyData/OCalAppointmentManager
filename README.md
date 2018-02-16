# OCal Appointment Manager

The library implements an Appointment Manager interface for the purpose of demonstrating the features of the Brainy Data OCal external component.

To build the library you will require the OCal external components by Brainy Data. If you do not have it, demo versions are available at https://www.brainydata.com/demos.

The specific downloads are:

https://www.brainydata.com/demos/software/ocal_demo_software_mac.zip
https://www.brainydata.com/demos/software/ocal_demo_software_win.zip

Please refer to the online documentation for further information.
https://www.brainydata.com/supportpublic/documentation.htm

## Contents

### OCalAppointmentManager

This folder contains the JSON source files for the Omnis library in Github.

To restore these files in Omnis Studio, click 'Libraries' in the Studio Browser, then click 'New Lib from JSON'. In the import dialog, navigate to this source folder (containing library.json), then specify a different location for the new Library. Click on Import and open the library in the Studio Browser.

### Known Issues

OCal overrides the build-in property $vertscroll. However, this currently does not work correctly during export or import of JSON. We have fixed the exported source manually, but until this issue is resolved, after importing the JSON, the OCal objects on the window wGroupView require manual fixing. For all but the last OCal object on this window, the $vertscoll property should be set to kFalse. We have reported this issue to Omnis Software and they are investigating.
