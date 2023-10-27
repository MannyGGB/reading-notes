# Class 05 (27/10/2023)

## Morning challenge

/_ given an array of player objects, each with a name and a score. Your task is to filter out players who have a score less than 80. _/

const players = [
{ name: 'Alice', score: 90 },
{ name: 'Bob', score: 85 },
{ name: 'Charlie', score: 92 },
{ name: 'David', score: 78 },
{ name: 'Eve', score: 95 },
{ name: 'Frank', score: 50 },
{ name: 'Sam', score: 89 }
];
let newPlayers = players.filter(function(players) {
players.score < 80 ? console.log(players) : console.log("none")
})

const filteredPlayers = players.filter(player => player.score >= 80)
console.log(filteredPlayers)

/_ Stretch Goal: sort the remaining players by their score in descending order then only console.logging the top 3 players _/

      const sortedPlayers = filteredPlayers.sort((a,b) => b.score - a.score)
        console.log

const top3 = sortedPlayers.splice(0,3)
console.log(top3)

## Lab recap

- Add form and different solutions to filter()

## Browser Router

- Demo repo

## Vercel

- Set up account
