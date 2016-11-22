The `adm` directory contains multiple files that provide slightly different policies:
  * `SearchProviderEcosia.adm`: Provides Ecosia as search engine
  * `SearchProviderEcosiaBing.adm`: Provides Ecosia and Bing as search engines
  * `SearchProviderEcosiaBingGoogle.adm`: Provides Ecosia, Bing and Google as search engines

To use the templates follow these steps:
  1. Open the _Group Policy_ administration tool. You can start _group policy editor_ by typing `gpedit.msc` into the _Windows command_ bar
  2. Depending on the target of your policy (`LOCAL_MACHINE` or `CURRENT_USER`), expand either the _Computer Configuration_ or _User Configuration_ file browser
  3. Right-click on the _Administrative Templates_ folder and select "_Add/Remove Templates_"
  4. Click the "_Add…_" button and select the desired _SearchProvider.adm_ file from the `adm` folder
  5. To enable the new policy, expand the _Administrative Templates_ folder and enable: Administrative Templates\Classic Administrative Templates (ADM)\Windows Components\Internet Explorer\Populate List of search providers
  6. Choose which search engines you would like to add (the options will differ depending on which policy file you selected in step 4) and click "Apply"
  7. After applying the new search engines, you must edit an additional policy for Internet Explorer by following one of the steps below:
    1. To enable the search engines added in step 6, but still allow users to modify their search engines list, enable the policy: Administrative Templates\Windows Components\Internet Explorer → Add a specific list of search providers to the user’s list of search providers
    2. To enable the search engines added in step 6 and restrict the IE search engine list to those selected in step 4, enable the policy: Administrative Templates\Windows Components\Internet Explorer → Restrict Search providers to a specific list
