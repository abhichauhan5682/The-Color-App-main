# Getting Started with Create React App

## Live Demo: [Demo](https://the-color-app.netlify.app/)

#                                            PROJECT : COLOR PICKER
## This project is build up by using frontend framework call REACTJS. 

## Different libraries are used to make things easy
### 1)Chroma-js
Chroma.js is a small-ish zero-dependency JavaScript library (13.5kB) for all kinds of color conversions and color scales.
### 2)rc-slider
It is used to build slider in our navbar with the help of this slider we can different type of level for a single color
### 3)react-copy-to-clipboard
It is used to copy the name of the color by clicking on respective color
### 4)@material-ui
It is the popular interface library for reactjs we can use different types of component’s which is already built in material-ui we just have to import in our file such as Button ,Select ,Dialog-box, Drawer etc. 
### 5)@material-ui/styles
With the help of this library we can write our css in to our js files
With the help of this we can use conditional operator for styling our page, for eg: props=>chroma(props.background).luminance()>=0.7 ?"rgba(0,0,0,0.6)":"white",
### 6)react-ui/form-validator
To validate the form to check whether new typed color is unique or not or selected color is unique or not
### 7)react-color
With the help of this we can import chromePicker in to our file and we can select colors to add into new palette
### 8)react-sortable-hoc
It is the library used to drag-n-drop new colors which is added into our new palette. Therefore user’s can order them in their way.


## Seedcolor.js
It contains an array  which is used to provide initial colors to our palette

## colorhelper.js
it is used to provide single object which contain colors of different level. Each level contains an array and each entry in an array is an object which has id, name ,hex, rgb, 
rgba.
Chroma js library is used to build color in different levels.
Levels used are:{50,100,200,300,400,500,600,700,800,900}

## Different types of Component made to build to this project

### 1)App.js (Class Component):
It is the epicenter of our project  and controls various components according to routes
Different Routes are used:
    1)	“/” to show list of palettes , It renders PaletteList component
    2)	“/palette/:paletteid” to show single palette , It renders Palette component
    3)	“/palette/new” to show from for to make new palette, It renders NewPalette component
    4)	“/palette/paletteid/colorid” to show various levels for single color , It renders singleColor component.
### 2) Pallete.js (Class Component): 
to show single palette and a navbar. Navbar contains slider and dropdown which is used to change the level of the colors (100,200,..900) of palette and the type (hex , rgb, rgba) respectively .

![image](https://user-images.githubusercontent.com/58387831/104203871-a3609780-5452-11eb-8454-6531f2c2c0ba.png)
 
### 3)Color.js : (Class Component):
It is used to show a single color in our palette each color contains its name and its level , more button which is used to show various level of single color and copy button which is used to copy the color. The copy button shows only when we hover on the color.

![image](https://user-images.githubusercontent.com/58387831/104204032-d1de7280-5452-11eb-8844-f4f8c4c722d0.png)

 
### 4)Singlecolor.js : (Class Component):
to show different levels of single color present in the palette. It is rendered when we click more button . it also show navbar which contains a dropdown to select type of color i.e hex , rgb or rgba.

![image](https://user-images.githubusercontent.com/58387831/104204132-f1759b00-5452-11eb-8038-13ea8ac1cf70.png)
 
### 5)PaletteList.js (Class Component) :
It is used to show list of palettes . It is our initial page of our project. It show minified version of our palette .

![image](https://user-images.githubusercontent.com/58387831/104204211-05210180-5453-11eb-8663-7f6597e52ff1.png)
 
### 6)MiniPalette.js (Class Component): 
It is used to show the minifed version of our palette into our initial page. It shows the palette name and the emoji and the color used in our palette. It also show delete icon to delete the palette from the list when we hover on the minipalette

 ![image](https://user-images.githubusercontent.com/58387831/104204262-1407b400-5453-11eb-94e5-6def3c6a365a.png)

### 7)NewPalette.js (Class Component):
It is rendered when we click create palette in our front page. It show us the COLOR PICKER FORM to add new color to our new Palette. Initially it contains 19 colors we can delete these colors add our own colors. This page is made from Drawer Component(material-ui).  We can also hide our color picker form.

![image](https://user-images.githubusercontent.com/58387831/104204307-22ee6680-5453-11eb-945f-80b67931c508.png)

![image](https://user-images.githubusercontent.com/58387831/104204338-2f72bf00-5453-11eb-86b7-0e6cc2b6ce41.png)

### 8)Colorpicker.js (Class Compoment): 
It is used in our NewPalette component  to show colorpicker form . We used react-color library to include Chrome Picker in our component.
We also used react-ui-form-validator to validate our form. For examples : to check whether color and color-name is unique and to check before submitting the form input value is not empty.
It also contains 2 buttons one to clear palette and one to add random color which is not used in our palette. 
It also alert when our palette is full and we try to add new color by changing the text of ADD COLOR button to PALETTE IS FULL
    
![image](https://user-images.githubusercontent.com/58387831/104204429-49ac9d00-5453-11eb-9a1c-19c357e255b8.png)
![image](https://user-images.githubusercontent.com/58387831/104204449-4fa27e00-5453-11eb-9062-99f776bc43a2.png)
![image](https://user-images.githubusercontent.com/58387831/104204472-54673200-5453-11eb-80e1-4aa0d255856b.png)
![image](https://user-images.githubusercontent.com/58387831/104204488-592be600-5453-11eb-9899-6b29219a2567.png)
![image](https://user-images.githubusercontent.com/58387831/104204509-5cbf6d00-5453-11eb-975c-ef4f4f5691f1.png)
   



# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.\
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)
