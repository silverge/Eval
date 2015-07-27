HOW TO

In order to run this plugin and see the results, you must put the plugin file, a text file and the corresponding html file into one folder in Orionhub.org
The plugin file must be opened as a website and the url must be saved. You can do this by selecting the intended file and upon right clicking the file, select Open With -> Web Browser.
In the settings tab of Orion, the 'install' button is clicked and the url is inserted. On the source file, all of the corresponding occurences of 'eval' and/or 'apply' should be underlined in yellow. When you hover on that word, it should show you the eval traces corresponding to that line.

Here are the matches of traces and source files with plugins:

Berts-BreakdownEval.txt and bertsSource.html --> EvalPlugin.html and UpdatedEvalPlugin.html 

applyR.txt and applyS.html --> Apply&EvalPlugin.html

eval&array.txt and eval&array.html --> Apply&EvalPlugin.html

***make sure the correct trace (text) file is supplied in the plugin.

--> in the line where it says: xmlhttp.open("GET","eval.txt", false); 
