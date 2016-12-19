The `admx` directory contains the main `admx` file together with its language resources (in the folder `en-US`). 

To use the template follow these steps:
  1. Copy the `admx` file together with the `en-US` folder to the correct place:
    * Local: `%systemroot%\policyDefinitions` (normally `C:\Windows\policyDefinitions`)
    * Domain: `%systemroot%\sysvol\domain\policies\PolicyDefinitions` (normally `C:\Windows\sysvol\domain\policies\PolicyDefinitions`)
  2. Open the _Group Policy_ administration tool. You can start _group policy editor_ by typing `gpedit.msc` into the _Windows command_ bar
  3. Depending on the target of your policy (`LOCAL_MACHINE` or `CURRENT_USER`), expand either the _Computer Configuration_ or _User Configuration_ file browser
  4. Navigate to _Administrative Templates_ → _Ecosia_ → _Google Chrome_ → _Default search provider_
  5. Enable all desired options
    * All options already have the correct default values to work with Ecosia
    * Keep in mind that _Enable the default search provider_ has to be enabled for any of the other options to take effect
