# Sergey Zenkovich

## Contact Info:
* Telegram  - https://t.me/SergeyZenkovich
* Mobile - +375298868275 
* E-mail - sapocalipsys.z@gmail.com
* Skype - sergeyilsk
* LinkedIn - https://www.linkedin.com/in/sergey-zenkovich-2a0a72183

## Summary:
 I am researcher in GIS and remote sensing areas. In 2019 I graduated from the University(BSU - geography faculty - GIS specialist). Now I am working with spatial data, analyzing space images, writing scripts for GIS software environment(Python). For me it's interesting to try out FrontEnd. I have some experience in FrontEnd (completed courses: “FrontEnd start” in TeachMeSkills, “ServiceNow” in EPAM; tried: “RSSchool-2019/2020” ). My goal is to improve my skills in FrontEnd and interconnect my knowledge on GIS and spatial data analyzing and FrontEnd in my future job.<br/> 
**Wishes:**
 * Improve hard skills.
 * Work in future with AR and VR technologies.
 * Try myself in web design. 

## Hard Skills:
* HTML5 + semantic HTML
* CSS + Sass + Less
* ES 5 + ES next
* BEM methodology
* JQuery
* Bootstrap
* Git
* Webpack
* React
* Redux
* Material UI
* Phyton 
* SQL

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
```Javascript
import { useEffect, useState } from 'react';
import './App.css';
import InputToDo from './Components/InputToDo';
import ListComponent from './Components/ToDoList';
import db from './firebase';
import firebase from 'firebase'

function App() {

  const [todos, setTodos] = useState([]);

  useEffect(()=>{
    db.collection('todos').orderBy('timestamp','desc').onSnapshot(snapshot=>{
      setTodos(snapshot.docs.map(doc=> ({id:doc.id, todo: doc.data().todo})))
    });
  },[])

  const addTodoTask = (task)=>{
    db.collection('todos').add({
      todo: task,
      timestamp: firebase.firestore.FieldValue.serverTimestamp()
    });

    setTodos((prev)=>{
      return [...prev, task];
    })
  }
  
  return (
    <div className="App">
      <h1>ToDo App</h1>
      <InputToDo addTodoTask = {addTodoTask}/>
      <ListComponent tasks = {todos}/>
    </div>
  );
}

export default App;
```
## Experience:
 No working experience (only self coding and courses projects).
## Education:
* Online courses and Tutorials (HTML Academy, Codeacademy, The Modern JavaScript Tutorial).
* completed courses: “FrontEnd start” in TeachMeSkills, “ServiceNow” in EPAM;
* tried: “RSSchool-2019/2020”; 
## English:
 **B1 level** (have certification of "Ispeek" language school) Keep learning.
