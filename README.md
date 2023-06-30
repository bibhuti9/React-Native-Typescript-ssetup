# React-Native-Typescript-ssetup


#packages for this project
  react-native-config
  1. HOC
  2. Theme
  3. redux
  4. mobx
  5. navigation
     a. Drawer
     b. Bottom tab
     c. Top tab 
  7. API
     a. setup standard method   
  9. Firebase
  10. Localstorage
  11. Authontication

|| --------------- Todo App ------------- ||

  1. Search
  2. List all notes
  3. At bottom add fab action
  4. bottom tab (custom)
     a. Home
     b. User
  6. Drawer (customaa )
  7. Editor / Add


---------------- FLOW --------------------------

/*

1. Entry point
2. Navigation
3. Theme provider
4. Authontication
5. Enviroment variable
6. Structure
    utils
    component
    store
    screens
    navigation
    theme
    assets
    api
7. API

*/
  


react-native-config
moment
mobx
mobx-react
mobx-state-tree

@react-native-community/netinfo
"@react-native-firebase/app": "^16.5.2",
"@react-native-firebase/auth": "^16.5.2
"@react-native-firebase/messaging": "^16.5.2",
react-native-permissions


````
```

------------------------- ADD Aliasing --------------------------


 Goto => tsconfig.json
   // ... other configs, if any
    "compilerOptions": {
       // ... other configs, if any
       "baseUrl": "." ,
       "paths": {
          "@api/*": [
            "src/api/*"
          ],
          "@utils/*": [
            "src/utils/*"
          ]
       },
    }

Install yarn add --dev babel-plugin-module-resolver

# code
Goto => babel.config.js 
  plugins: [
    // ... other configs, if any
    [
      'module-resolver',
      {
        extensions: ['.ios.js', '.android.js', '.ios.jsx', '.android.jsx', '.js', '.jsx', '.json', '.ts', '.tsx'],
        root: ['.'],
        alias: {
          '@api': './src/api',
          '@assets': './src/assets',
          '@components': './src/components',
          '@scenes': './src/scenes',
          '@theme': './src/theme',
          '@utils': './src/utils',
        },
      },
    ],

    // ... other configs, if any
  ],
  

```
````
  
 
