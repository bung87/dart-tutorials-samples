![script tags](./script-tags.png)  
The first script includes your mini app. The `type` attribute specifies that the script has the type `application/dart`, which is a new type created by the Dart team. Currently, only the Dartium build of Chromium supports `application/dart`. The `src` attribute provides the URL to the source file of the script. In this case, it is the Dart source file `mini.dart`, which you provide in the next step. The Dart file should be in the same directory as its host HTML file.

The second `script` tag is a bootstrap script that takes care of turning on the Dart VM, as well as compatibility with non-Dart browsers.
