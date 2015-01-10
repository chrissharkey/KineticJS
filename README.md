# Documentation for KineticJS

# How to help?

You can see old tutorials here: [Archive](https://web.archive.org/web/20131218201507/http://www.html5canvastutorials.com/kineticjs/html5-canvas-kineticjs-path-tutorial)

Now we need to copy all of them to current site. All files for generation stored inside `docs` folder.

For example if you want to create tutorial for "Drag events":

1. Create folder `Drag and Drop` inside `docs` if it does not exist. 
2. Create file `01_Drag_events.md`.
3. Type somithing important inside file.
4. You can embed code with any "fiddle" service. I prefer JSbin. You can use this bin for tempale: [http://jsbin.com/bipoke/1/edit?html,js,output](http://jsbin.com/bipoke/1/edit?html,js,output). Just change "title" and "description" inside html, and edit the code. Then get embed code via "share" button.
5. You can insert code simply inside `01_Drag_events.md` file. I will create fiddle by myself.
6. Create pull request to gh-pages branch.
7. I may generate pages by myself.
8. Be happy.


## How to generate?

 1. Update files inside ./docs
 2. run ./build.sh