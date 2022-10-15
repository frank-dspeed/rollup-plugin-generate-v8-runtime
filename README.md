# rollup-plugin-generate-v8-runtime
Creates small v8 runtimes out of rollup bundels 

## Why?
V8 does not include a real module system there exist many interfaces to build modules builtIns and other stuff for v8 all that is also cluttered as it got a lot of historical bloat that is not needed anymore today.

i think it is a good integration point to offer for developers this way you can combine .js with nativ code in a easy way and directly bundle it into a v8::isolate instance that allows you to create indipendent workers that can spawn own workers.

this concept is also used extensiv in https://github.com/stealify and that is also the reason why this exists. if you need some compatible modules you will mostly find them there. or you can contribute them there. 
