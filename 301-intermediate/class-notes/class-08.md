# Class 08 (01/11/2023)

## Morning Challenge

When I click on the button, the image shows or disappears.

import './App.css'
import {useState} from "react"
export default function App() {
const [image, setImage] = useState(false)

function handleImage(){
setImage(!image)
}
return (

<main>
<button onClick={handleImage}>Show/Hide Image</button>
{image && <img src="http://placekitten.com/200/300"/>}
</main>)}

---

// random image when clicking
import {useState} from "react"

export default function App() {
const [showImg, setShowImg] = useState(false)
const [url, setUrl] = useState("")

function handleClick() {
setShowImg(!showImg)

    let h = Math.floor(Math.random() * 200) + 100;
    let w = Math.floor(Math.random() * 200) + 200;
    setUrl(`http://placekitten.com/${w}/${h}`);

}

return (

<main>
<button onClick={handleClick}>Show/Hide Image</button>
<br />
{showImg && <img src={url}/>}
</main>
)
}

## APIs

Nodemon server --> it updates the server whenever there is a change, so we don't have to stop and start the server after every change.
npm i cors express dotenv nodemon

- Create a WRRC graphic to show the requests and responses between client and server or servers.

Vercel.com --> host front end
Render.com --> host back end
