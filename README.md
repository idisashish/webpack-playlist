# webpack-playlist - SASS Loader

- install node-sass, sass-loader
- - npm install node-sass sass-loader --save

# change webpack.config
{
 test: /\.scss$/,
 loader: 'style-loader!css-loader!sass-loader'
}

- sass-loader -> converts .scss into .css
- css-loader -> will load css into .js
- style-loader -> will apply css to DOM
