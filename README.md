Steps to complete project - 
1 - book said to import the "initial" project, providing a skeleton to work from. 
![initialproject](https://user-images.githubusercontent.com/37083055/177229778-9a2026cd-f41e-4475-8967-57ea651fbb4e.png)
2 - knowing we would need the Musixmatch API, I created a username and password to the site. I then got a valid API key. Then I went to the api-key.ts and applied the key to the code. This will allow us to leverage the API later.
![CreateandImplimentAPIKey](https://user-images.githubusercontent.com/37083055/177229751-9473d3b3-075b-43c2-94a5-d5aae6996de1.png) 
3 - we then need to finish completing the InversifyJS setup. InversifyJS lets us use a class constructor to inject dependencies. We do so by using decorators to make the class conductors injectable. 
![InversifyJS Setup](https://user-images.githubusercontent.com/37083055/177230348-b2672318-54d9-4c36-aa2d-36441290e0aa.png)
4 - Next we added the code to create a skeleton view in the views/Home.vue file. This will contain many of our elements that will be part of the application that is viewable to others access the page. This will be built out in future steps. 
![BasicPageSetup](https://user-images.githubusercontent.com/37083055/177230656-66e2694f-7621-4dd2-8dd8-b009a32e5615.png)
5 - We need to setup our vue router, which is the library for simple page navigation. We install normally then make changes to multiple files. Ultimately, we see that the changes in the Home.vue file get routed and displayed in the App.vue page by simply applying the <router-view> tag.  
![VueRoutersetup](https://user-images.githubusercontent.com/37083055/177231105-6aeb9b82-45c5-4c00-8161-902a2d451995.png)
6 - We then import the Element.Ui library to give us an improved UI toolset to work from. With the next step being importing code from the book that leverages that library and css containers to better organize the App.vue page. 
![ElementImport](https://user-images.githubusercontent.com/37083055/177231346-6e71061e-2068-4129-ae40-eb29f5e44af8.png)
7 - Now that we have the needed page setup components to enable inputs, we must create the components that leverage the Musixmatch API to find artists and lyrics when typed into the search bar. This code was mostly given to us by the book. However, we do get to use Vue slots which allow for content projects like artists in this case onto the page. 
![SearchComponent](https://user-images.githubusercontent.com/37083055/177231705-45b9b67c-830c-4881-8244-ba4bd411325a.png)
8 - Leveraging InversifyJS, we inject the MusicService component and add event handlers to manage cache clearing. 
9 - Next, we build out the song list component better to enable display and song lyrics fetching from the two components. We also leverage the best practice construction of the CSS from the Element UI library. 
![SongList Component](https://user-images.githubusercontent.com/37083055/177232380-3d196c15-461c-4a13-9888-7c456faedf96.png)
10 - We now create the file, route, and enable the lyrics of selected songs to be displayed within our application when the event to do so occurs. This inludes using the view-router from the previous step.
![lyricsdisplay](https://user-images.githubusercontent.com/37083055/177232670-37b1a70a-e553-486e-84f1-83708bc8ed0c.png)
![lyricsdisplay2](https://user-images.githubusercontent.com/37083055/177232704-6176aefd-041b-4a4b-bf73-3c11b3f8d888.png)
11 -  We now have a finished application per the book 
![application](https://user-images.githubusercontent.com/37083055/177232779-ca7208ce-0769-43b0-ba9b-99bbca2b769f.png)

# Vue TS

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Run your tests
```
npm run test
```

### Lints and fixes files
```
npm run lint
```

### Run your end-to-end tests
```
npm run test:e2e
```

### Run your unit tests
```
npm run test:unit
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
