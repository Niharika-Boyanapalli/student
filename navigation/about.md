---
layout: post
title: About Me
permalink: /about/
comments: true
---

## As a conversation Starter

Here are some places I have lived.

<comment>
Flags are made using Wikipedia images
</comment>

<style>
    /* Style looks pretty compact, 
       - grid-container and grid-item are referenced the code 
    */
    .grid-container {
        display: grid;
        grid-template-columns: repeat(auto-fill, minmax(150px, 1fr)); /* Dynamic columns */
        gap: 10px;
    }
    .grid-item {
        text-align: center;
    }
    .grid-item img {
        width: 100%;
        height: 100px; /* Fixed height for uniformity */
        object-fit: contain; /* Ensure the image fits within the fixed height */
    }
    .grid-item p {
        margin: 5px 0; /* Add some margin for spacing */
    }

    .image-gallery {
        display: flex;
        flex-wrap: nowrap;
        overflow-x: auto;
        gap: 10px;
        }

    .image-gallery img {
        max-height: 150px;
        object-fit: cover;
        border-radius: 5px;
    }
</style>

<!-- This grid_container class is used by CSS styling and the id is used by JavaScript connection -->
<div class="grid-container" id="grid_container">
    <!-- content will be added here by JavaScript -->
</div>

<script>
    // 1. Make a connection to the HTML container defined in the HTML div
    var container = document.getElementById("grid_container"); // This container connects to the HTML div

    // 2. Define a JavaScript object for our http source and our data rows for the Living in the World grid
    var http_source = "https://upload.wikimedia.org/wikipedia/commons/";
    var living_in_the_world = [
       
    {"flag": "0/01/Flag_of_California.svg", "greeting": "Hey", "description": "California - forever"},
    {"flag": "8/88/Flag_of_Australia.svg", "greeting": "G’day", "description": "Australia - 1 year"},
    {"flag": "4/41/Flag_of_India.svg", "greeting": "Namaste", "description": "India - 6 months years"},
    {"flag": "3/3e/Flag_of_New_Zealand.svg", "greeting": "Kia ora", "description": "New Zealand - 6 months"}
]
    // 3a. Consider how to update style count for size of container
    // The grid-template-columns has been defined as dynamic with auto-fill and minmax

    // 3b. Build grid items inside of our container for each row of data
    for (const location of living_in_the_world) {
        // Create a "div" with "class grid-item" for each row
        var gridItem = document.createElement("div");
        gridItem.className = "grid-item";  // This class name connects the gridItem to the CSS style elements
        // Add "img" HTML tag for the flag
        var img = document.createElement("img");
        img.src = http_source + location.flag; // concatenate the source and flag
        img.alt = location.flag + " Flag"; // add alt text for accessibility

        // Add "p" HTML tag for the description
        var description = document.createElement("p");
        description.textContent = location.description; // extract the description

        // Add "p" HTML tag for the greeting
        var greeting = document.createElement("p");
        greeting.textContent = location.greeting;  // extract the greeting

        // Append img and p HTML tags to the grid item DIV
        gridItem.appendChild(img);
        gridItem.appendChild(description);
        gridItem.appendChild(greeting);

        // Append the grid item DIV to the container DIV
        container.appendChild(gridItem);
    }
</script>

### Journey through Life

Here is my life so far!!!
<<<<<<< HEAD
- 
=======
- 🏫 Lots of Elementary Schools in Del Sur, San Diego, (CA)
- 🏫 Middle and High School in Del Sur (CA)
- 🎓 I love math and computer science!
- ⛪ II play competetice club soccer!
>>>>>>> e539b4e292ce0108c50af3345c2c1b166ee78f9a

### Culture, Family, and Fun

Everything for me, as for many others, revolves around family and faith.

- I am australian, for i have australian citenzenship. My mom studied in a private unibversity in New Zealand so I also have citenzenship there.
- My dad studied at clemson, and loves watching his football team play college ball.
- I play soccer ECNL, and my team, Surf, won the National Championship back to back for the second year in a row.
- I hope to pursue Aerospace engineering and Computer Science for my dream job.


<comment>
Gallery of Pics, scroll to the right for more ...
</comment>
<div class="image-gallery">
<<<<<<< HEAD

=======
  

