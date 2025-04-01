# expo-bun-reproducable

1. Step 1
   `bun upgrade` to get the latest version of bun (1.2.8)
2. Step 2
   `bun create expo my-app` to create an expo app
# Result
```
╭─    ~/dev/expo ··············································   11:40:58 am
╰─❯ bun create expo my-app
Creating an Expo project using the default template.

To choose from all available templates pass in the --template arg:
  $ bunx create-expo --template

To choose from all available examples pass in the --example arg:
  $ bunx create-expo --example

✖ Something went wrong in downloading and extracting the project files: Executable not found in $PATH: "npm"
Error: Executable not found in $PATH: "npm"
63 |
64 |     {bold  npm:} {cyan npx ${d.CLI_NAME}}
65 |     {bold yarn:} {cyan yarn create ${t}}
66 |     {bold pnpm:} {cyan pnpm create ${t}}
67 |     {bold  bun:} {cyan bun create ${t}}
68 |     `)}const{AnalyticsEventPhases:a,AnalyticsEventTypes:l,flushAsync:v,track:E}=await Promise.resolve().then((()=>u(i(4575))));try{const h=await(0,b.resolveStringOrBooleanArgsAsync)(t,r,{"--template":Boolean,"--example":Boolean,"-t":"--template","-e":"--example"});w(`Default args:\n%O`,o);w(`Parsed:\n%O`,h);const{createAsync:d}=await Promise.resolve().then((()=>u(i(1961))));await d(h.projectRoot,{yes:!!o["--yes"],template:h.args["--template"],example:h.args["--example"],install:!o["--no-install"]});E({event:l.CREATE_EXPO_APP,properties:{phase:a.SUCCESS}});await v()}catch(t){if(!(t instanceof p.ExitError)){g.Log.exception(t)}E({event:l.CREATE_EXPO_APP,properties:{phase:a.FAIL,message:t.cause}});await v().finally((()=>{process.exit(t.code||1)}))}finally{const t=await(await Promise.resolve().then((()=>u(i(5897))))).default;await t()}}run()},9247:(t,r,i)=>{"use strict";Object.defineProperty(r,"__esModule",{value:true});r.CLI_NAME=void 0;r.CLI_NAME=i(4147).name},1961:function(t,r,i){"use strict";var o=this&&this._ | ... truncated

TypeError: The "code" argument must be of type number. Received type string ('ENOENT')
 code: "ERR_INVALID_ARG_TYPE"

      at <anonymous> (/private/tmp/bunx-501-create-expo@latest/node_modules/create-expo/build/index.js:68:736)

Bun v1.2.8 (macOS arm64)
```
