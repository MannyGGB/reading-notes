# Class 12 (03/10/2023)

## Lab review

- demo.js in project

## JS Libraries

- We add libraries to borrow code.
- We use a CDN to add the library to our HTML. We use the script tag with src. The CDN goes in src.

### Chart JS

- Library to make graphs into your website.
  const ctx = document.getElementById("my-chart");
  new Chart(ctx, {
  type: "bar",
  data: {
  labels: ["Jurassic Park", "Life of Brian", "Galaxy Quest", "Lord of the Rings", "Chicken Run"],
  datasets: [{
  label: "# of votes",
  data: [1, 2, 3, 4, 5],
  borderWidth: 6,
  backgroundColor: ["red", "yellow", "skyblue", "green", "orange"]
  }

  ]
  }
  })

## HTML canvas

- We use it to draw on it.
- <canvas id="my-canvas"></canvas>
