# Class 07 (31/10/2023)

## Morning Challenge

export default function App() {
const [number, setNumber] = useState(0)

function increaseNum() {
setNumber(number + 1)
}
function decreaseNum() {
setNumber(number - 1)
}
return (
<main>
<button onClick={decreaseNum}>-</button>
<span>{number}</span>
<button onClick={increaseNum}>+</button>
<p>When I press the + and - button, the number goes up and down.</p>

    </main>

)
}

## Express Servers

- cors --> bridge between client and server, so they can communicate. Cross Origin Resource Sharing
- Terminal:
  - npm init -y (for default answers)
  - npm i express cors dotenv (installs 3 server packages)
  - npx kill-port 8080 --> when the server can't use the port, kill all ports and do node server again
  - node server --> show server on browser
