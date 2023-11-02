# Class 09 (02/11/2023)

## Full-stack app demo using APIs (mono repo)

~ cd projects
➜ projects mkdir translatim
➜ projects cd translatim
➜ translatim npm create vite@latest
✔ Project name: … client
✔ Select a framework: › React
✔ Select a variant: › JavaScript

Scaffolding project in /home/manny/projects/translatim/client...

Done. Now run:

cd client
npm install
npm run dev

➜ translatim cd client
➜ client ..
➜ translatim mkdir server
➜ translatim ls
client server
➜ translatim cd server
➜ server touch server.js
➜ server ls
server.js
➜ server npm init -y
Wrote to /home/manny/projects/translatim/server/package.json:

{
"name": "server",
"version": "1.0.0",
"description": "",
"main": "server.js",
"scripts": {
"test": "echo \"Error: no test specified\" && exit 1",
"start": "node server.js"
},
"keywords": [],
"author": "",
"license": "ISC"
}

➜ server ls
package.json server.js
➜ server npm i express cors dotenv nodemon axios

added 105 packages, and audited 106 packages in 2s

16 packages are looking for funding
run `npm fund` for details

found 0 vulnerabilities
➜ server cd ..
➜ translatim code .
➜ translatim

---

➜ translatim git init
Initialized empty Git repository in /home/manny/projects/translatim/.git/
➜ translatim git:(main) ✗ git remote add origin git@github.com:MannyGGB/translatim.git
➜ translatim git:(main) ✗ git add .
➜ translatim git:(main) ✗ git commit -m "Initial commit"
➜ translatim git:(main) git push

---

vercel
make sure vite is ticked and root is set to client

---

render
name = project name
region = EU
root directory = server
runtime = node
build command = npm i
start command = node server
