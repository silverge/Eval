Orion Research

Since this is an open source framework, there are several contributors that update and modify Orion’s code. It’s helpful to have the right people to ask if you run into trouble or what to know more about the developing environment.

Orion developer discussion mailing list: https://dev.eclipse.org/mailman/listinfo/orion-dev

All the source code for Orion is on GitHub: https://github.com/eclipse/orion.client
You can find the Orion Documentation/ Developer Guide on the following page: https://wiki.eclipse.org/Orion/Documentation/Developer_Guide

Orion Plugins: is an HTML file containing some JavaScript that knows how to connect to the Orion client. Plugins can be hosted on any web server and installed into Orion using their URL.
Here is the link to a useful page that shows what you need for a plugin and gives a simple example of an Orion plugin: https://wiki.eclipse.org/Orion/Documentation/Developer_Guide/Simple_plugin_example

orion.edit.contentAssist: Orion provides an extension point to allow plugins to define alternative implementations of content assist. The Content Assist service contributes content assist providers to the editor. A content assist provider produces suggestions for text that may be inserted into the editor at a given point. Content assist is a key class for implementing the code completion functionality. 
Here is the current code to content assist: http://git.eclipse.org/c/orion/org.eclipse.orion.client.git/tree/bundles/org.eclipse.orion.client.javascript/web/javascript/contentAssist

Here is a useful link to the documentation for Content Assist the with example plugins: https://wiki.eclipse.org/Orion/Documentation/Developer_Guide/Plugging_into_the_editor#orion.edit.contentAssist

orion.edit.validator: The validator service provides a function that can check the contents of a file and return a data structure indicating where problems are. The result of this service is used by the Orion UI to create annotations in the ruler beside each problematic line, and also to underline the specific portion of the document where the problem occurs.

We used this validator service to underline all instances of eval and show what the eval function was doing. 
Here is a useful link to the documentation for Content Assist the with example plugins: https://wiki.eclipse.org/Orion/Documentation/Developer_Guide/Plugging_into_the_editor#orion.edit.validator

XMLHttpRequest: object was used in order to convert the given text file into a string. The XMLHttpRequest object allows for a data exchange with the server after the page has loaded. The methods used were open, send and responseText. First, the text file was inputted and sent to the server, then the data received was turned into a string.
Here is a useful link to help show the methods used and their parameters: http://www.w3schools.com/xml/xml_parser.asp

HOW TO

In order to run this plugin and see the results, you must put all the files into one folder in Orionhub.org
The eval plugin file must be opened as a website and the url must be saved. In the settings tab of Orion, the 'install' button is clicked and the url is inserted. On the source file, all of the corresponding occurences of 'eval' should be underlined in yellow. When you hover on that word, it should show you the eval traces corresponding to that line.
