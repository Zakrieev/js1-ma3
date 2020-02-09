// question 1
const sum = (a, b) => a - b;

// question 2

fetch("https://api.rawg.io/api/games?genres=sports")
    .then(function (response) {
        return response.json();
    })
    .then(function (json) {
        for (let i = 0; i < json.results.length; i++) {
            console.log(json.results[i].name);
        }
    })

    .catch(() => document.location.href = "error.html");


// question 3
let Wordreplace = "These cats are outrageous.";
Wordreplace = Wordreplace.replace("cats", "giraffes");

// question 4 
const queryString = document.location.search;
const params = new URLSearchParams(queryString);

let userId;

if (params.has("userId")) {
    userId = params.get("userId");
    const userIdNumber = parseInt(userId);

    if (userIdNumber < 10) {
        document.location.href = "first.html"
    } else if (userIdNumber >= 10) {
        document.location.href = "second.html"
    }

} else {
    document.location.href = "third.html"
}


// question 5
const container = document.querySelector(".container");
const button = document.querySelector(".btn");

container.removeChild(button);

// question 6

const list = document.createElement("li");
const listContent = document.createTextNode("Parrot");
list.className = "parrots";

list.appendChild(listContent);

listCow = document.querySelector(".cows");

listCow.appendChild(list);


// question 7

fetch("https://api.rawg.io/api/games/3801")
    .then(function (response) {
        return response.json();
    })
    .then(function (json) {
        const rating = document.querySelector(".rating");
        rating.appendChild(document.createTextNode(json.rating));
    })

    .catch(function (error) {
        console.log(error);
    });
