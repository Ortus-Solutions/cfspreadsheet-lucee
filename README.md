#&lt;cfspreadsheet /&gt; for Lucee

This is a fork of the Team CFAdvance cfspreadsheet-railo extension, modified to work with the Lucee fork of Railo. Please refer to that site for more details.

##Update:
The ApachePOI jars have been updated to the latest stable version (3.11)
xmlbeans-2.6.0.jar also added as per Apache recommendation, though v2.3 is all that is required.
Version bumped to 4.0 because of new jars.

##Installation: via Lucee Admin GUI

In this method, you will create your own temporary extension provider:

1. Download cfspreadsheet-lucee.zip
1. Extract into `/path/to/your/wwwroot/luceeExtensionProvider` (you should then have 2 files in that folder: cfpoi.zip and ExtensionProvider.cfc)
1. Add a file `/path/to/your/wwwroot/luceeExtensionProvider/Application.cfc` with the contents `component {}`
1. Lucee *Web* Admin > Extensions > Providers: Add:  `http://your_local_site_host/luceeExtensionProvider/ExtensionProvider.cfc` (ensure you are using the correct port in your setup)
1. Lucee *Web* Admin > Extensions > Applications:  Click on "&lt;cfspreadhsheet /&gt;" icon.
1. Click "Install" Button
1. Restart Lucee or Tomcat (depending on installation type)