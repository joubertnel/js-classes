JSPerf
======
http://jsperf.com/simple-define-instantiate-invoke/2


es6-transpiled.min.js
=====================
- Google Closure Compiler with ADVANCED_OPTIMIZATIONS turned on. 
- code executes correctly


utilClass.min.js
================
- utilClass with ADVANCED_OPTIMZATIONS generates 4 warnings (below)
- code fails to execute


utilClass.js:4: WARNING - dangerous use of the global this object
        this.title = title;
        ^

utilClass.js:5: WARNING - dangerous use of the global this object
        this.log = [];
        ^

utilClass.js:9: WARNING - dangerous use of the global this object
        this.log.unshift('Playing: ' + this.title);
        ^

utilClass.js:9: WARNING - dangerous use of the global this object
        this.log.unshift('Playing: ' + this.title);
                                       ^

0 error(s), 4 warning(s)


utilClass.min-simple.js
=============================
- Google Closure Compiler without ADVANCED_OPTIMAZATIONS
- code executes correctly
