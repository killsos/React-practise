## 1. 安装: npm install babel-cli -g
## 2. babel
* Compile Files
      babel script.js

* If you would like to output to a file you may use --out-file or -o.

      babel script.js --out-file script-compiled.js
      babel script.js -o script-compiled.js

* compile a file every time that you change it, use the --watch or -w option:

      babel script.js --watch --out-file script-compiled.js

* Compile Directories
* Compile the entire src directory and output it to the lib directory. You may use --out-dir or -d. This doesn’t overwrite any other files or directories in lib.

        babel src --out-dir lib

* Compile the entire src directory and output it to the one concatenated file.

        babel src --out-file script-compiled.js


* Ignore files

        babel src --out-dir lib --ignore spec.js,test.js

* Copy files

        babel src --out-dir lib --copy-files

* Piping Files

        babel --out-file script-compiled.js < script.js

* Using Plugins

        babel script.js --out-file script-compiled.js --plugins=es2015,react


* Using Presets

        babel script.js --out-file script-compiled.js --presets=add-module-exports,transform-es2015-modules-amd
