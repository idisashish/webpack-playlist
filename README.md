# webpack-playlist - Lesson 5 - CSS Loaders
## Why we need CSS Loaders
- Read this article- https://css-tricks.com/css-modules-part-1-need/  - This allows us to create module.css for each component like suppose we're working in React Component this would create a css style only for that component
- Go through Sonny Sangha - Styling Components

- Use CSS loaders to load in only the styles we need, into different parts of our application
- CSS becomes much more modular and easier to mangage

# CSS & STYLE Loaders

- 2 different loader - css-loader, style-loader
- Css-loader, loads the CSS into our JS file
- Style-loaders adds our css into the DOM

# Installing

npm install style-loader css-loader --save-dev

# 

module: { 
loaders:
  [ 
      { 
        test:/.js$/, 
        exclude: /(node_modules)/, 
        loader: 'babel-loader', 
        query: { presets: ['es2015'] 
      }, 
      {
        test: /\.css$/,
        loader: 'style-loader!css-loader'
      }
   } 
  ] 
}
