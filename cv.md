# Sergey Zenkovich

## Contact Info:
* Telegram  - https://t.me/SergeyZenkovich
* Mobile - +375298868275 
* E-mail - sapocalipsys.z@gmail.com
* Skype - sergeyilsk
* LinkedIn - https://www.linkedin.com/in/sergey-zenkovich-2a0a72183

## Summary:
 I am reseacher in GIS and remote sensing areas. In 2019 I graduated from the University(BSU - geography faculty - GIS specialist). Now I am working with spatial data, analyzing space images, writing some scripts for GIS program environment(Python). For me it is interesting to try out in FrontEnd. I have some experience in FrontEnd (completed courses: “FrontEnd start” in TeachMeSkills, “ServiceNow” in EPAM; try out: “RSSchool-2019(3)”). My goal is to improve my skills in FrontEnd and interconnect my knowledges of GIS and spatial data analyzing and FrontEnd in my future job.<br/> 
**Goal** - Work as a Front-End developer in a big product company. <br/>
**Wishes:**
 * Have strong knowledge in different frameworks.
 * Work in future with AR and VR technologies.
 * Try myself in web design. 

## Skills:
* HTML5 + semantic HTML
* CSS + Sass + Less
* ES 5 + ES next
* BEM methodology
* JQuery
* Bootstrap
* Git
* Webpack
* Phyton 
## Code examples:
```Javascript
	function swapHeadAndTail(arr) {
		const even = arr.length % 2 === 0;
		if (even) {
		 	 const firstHalf = arr.filter((elem, index) => index < arr.length / 2);
		 	 const secondHalf = arr.filter((elem, index) => index >= arr.length / 2);
		 	 return […secondHalf, …firstHalf]; 
		}
		const firstHalf = arr.filter((elem, index) => index < arr.length / 2 - 1);
		const middleElem = arr[Math.floor(arr.length / 2)];
		const secondHalf = arr.filter((elem, index) => index > arr.length / 2);
		return […secondHalf, middleElem, …firstHalf]; 
	}
```
```Javascript
	const path = require('path');
	const MiniCssExtractPlugin = require('mini-css-extract-plugin');
	module.exports = {
	  entry: ['babel-polyfill', './src/JS/index.js'],
	  output: {
	    path: path.resolve(__dirname, 'dist'),
	    filename: 'bundle.js'
	  },
	  module: {
	    rules: [
	      {
	        test: /\.(sa|sc|c)ss$/,
	        use: [
	          {
	            loader: MiniCssExtractPlugin.loader
	          },
	          {
	            loader: 'css-loader'
	          },
	          {
	            loader: 'postcss-loader'
	          },
	          {
	            loader: 'sass-loader',
	            options: {
	              implementation: require('sass')
	            }
	          }
	        ]
	      },
	      {
	        test: /\.js$/,
	        exclude: /(node_modules)/,
	        use: {
	          loader: 'babel-loader',
	          options: {
	            presets: ['@babel/preset-env']
	          }
	        }
	      },
	      {
	        test: /\.(png|jpe?g|gif|svg)$/,
	        use: [
	          {
	            loader: 'file-loader',
	            options: {
	              outputPath: 'images'
	            }
	          }
	        ]
	      },
	      {
	        test: /\.(woff|woff2|ttf|otf|eot)$/,
	        use: [
	          {
	            loader: 'file-loader',
	            options: {
	              outputPath: 'fonts'
	            }
	          }
	        ]
	      }
	    ]
	  },
	  plugins: [
	    new MiniCssExtractPlugin({
	      filename: 'bundle.css'
	    })
	  ],
	  mode: 'development'
	};
```
## Experience:
 No working experience (only self coding and courses projects).
## Education:
* Online courses and Tutorials (HTML Academy, Codeacademy, The Modern JavaScript Tutorial).
* completed courses: “FrontEnd start” in TeachMeSkills, “ServiceNow” in EPAM;
* tried: “RSSchool-2019(3)”; 
## English:
 **A2 level** (have certification of "Ispeek" language school) Keep learning.