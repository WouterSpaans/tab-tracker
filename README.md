# tab-tracker
Following a tutorial for learning Full Stack Web development with VueJS
Based upon tutorial found at: https://www.youtube.com/watch?v=Fa4cRMaTDUI

# Environment:

Things you'll need:

* [Visual Studio Code](https://code.visualstudio.com/docs/?dv=win)

* [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)

* [NodeJS](https://nodejs.org/en/download/)


## Setting up source code repository
```
cd C:\Users\Wouter\source\repos
git clone https://github.com/WouterSpaans/tab-tracker.git
cd tab-tracker
```

## Setting up VUE-CLI
```
npm install -g @vue/cli
vue create client
```

### Preset (content of ~/.vuerc)
```
{
  "presets": {    
    "Tutorial Preset 1": {
      "useConfigFiles": true,
      "plugins": {
        "@vue/cli-plugin-babel": {},
        "@vue/cli-plugin-typescript": {
          "classComponent": true,
          "useTsWithBabel": true
        },
        "@vue/cli-plugin-pwa": {},
        "@vue/cli-plugin-eslint": {
          "config": "standard",
          "lintOn": [
            "save"
          ]
        },
        "@vue/cli-plugin-unit-mocha": {},
        "@vue/cli-plugin-e2e-cypress": {}
      },
      "router": true,
      "vuex": true,
      "cssPreprocessor": "sass"
    }
  },
  "useTaobaoRegistry": false
}
```

```
git status
git add --all
git commit -m "init the vuejs application using vue-cli"
git push
```

# Start coding
```
cd client
npm run serve
```
* [Open localhost in browser](http://localhost:8080/#/)

Open visual studio code