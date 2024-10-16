<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dinosaurs by Myz</title>
    <style>
        body {
            font-family: 'Open Sans', sans-serif
        }
        .dinosaur {
            display: none; /* Hidden by default */
        }
    </style>
</head>
<body> 
    <banner>
      <img src="ee.jpg">
    </banner>
    <h1>
      <u>Dinosaurs</u>
    </h1>
      <p><b>Dinosaurs</b> are a diverse group of <b>reptiles</b> of the <b>clade Dinosauria</b>. They first appeared during the <b>Triassic period</b>, between <b>243 and 233.23 million years ago (mya)</b>, although the exact origin and timing of the <b>evolution of dinosaurs</b> is a subject of active research. They became the <b>dominant terrestrial vertebrates</b> after the <b>Triassic–Jurassic extinction event 201.3 mya</b> and their dominance continued throughout the <b>Jurassic</b> and <b>Cretaceous</b> periods. The fossil record shows that <b>birds are feathered dinosaurs</b>, <b>having evolved from earlier theropods during the Late Jurassic epoch</b>, and are the only dinosaur lineage known to have survived the <b>Cretaceous–Paleogene extinction event approximately 66 mya</b>. Dinosaurs can therefore be divided into <b>avian dinosaurs—birds</b> and the extinct <b>non-avian dinosaurs</b>, which are all dinosaurs other than birds.</p>
      <p>   Dinosaurs are varied from <b>taxonomic, morphological and ecological</b> standpoints. Birds, at over <b>11,000 living species</b>, are among <b>the most diverse groups of vertebrates</b>. Using <b>fossil evidence</b>, paleontologists have identified <b>over 900 distinct genera</b> and <b>more than 1,000 different species of non-avian dinosaurs</b>. Dinosaurs are represented on every continent by both <b>extant species (birds)</b> and fossil remains. Through the first half of the <b>20th century</b>, before <b>birds were recognized as dinosaurs</b>, most of the scientific community <b>believed dinosaurs to have been sluggish and cold-blooded</b>. Most research conducted since <b>the 1970s</b>, however, has indicated that <b>dinosaurs were active animals with elevated metabolisms and numerous adaptations for social interaction</b>. Some were <b>herbivorous, others carnivorous</b>. Evidence suggests that <b>all dinosaurs were egg-laying</b>, and that <b>nest-building</b> was a trait shared by many dinosaurs, both avian and non-avian.</p>
      <p>   While dinosaurs were <b>ancestrally bipedal</b>, many <b>extinct groups included quadrupedal species</b>, and some were able to <b>shift between these stances</b>. Elaborate display structures such as <b>horns or crests are common</b> to all dinosaur groups, and some extinct groups developed <b>skeletal modifications</b> such as <b>bony armor and spines</b>. While the dinosaurs' modern-day surviving avian lineage (birds) are generally small due to the <b>constraints of flight</b>, many prehistoric dinosaurs (non-avian and avian) were <b>large-bodied—the largest sauropod dinosaurs are estimated to have reached lengths of 39.7 meters (130 feet) and heights of 18 m (59 ft)</b> and were the <b>largest land animals of all time</b>. The <b>misconception that non-avian dinosaurs were uniformly gigantic</b> is based in part on <b>preservation bias</b>, as large, sturdy bones are more likely to last until they are <b>fossilized</b>. Many dinosaurs were <b>quite small, some measuring about 50 centimeters (20 inches) in length</b>.</p>
      <p>   The <b>first dinosaur fossils</b> were recognized in the <b>early 19th century</b>, with the name <b>"dinosaur" (meaning "terrible lizard")</b> being coined by <b>Sir Richard Owen in 1842</b> to refer to these <b>"great fossil lizards"</b>. Since then, <b>mounted fossil dinosaur skeletons</b> have been <b>major attractions at museums worldwide</b>, and dinosaurs have become an enduring part of popular culture. The large sizes of some dinosaurs, as well as their seemingly monstrous and fantastic nature, have ensured their regular appearance in best-selling books and films, such as the <b>Jurassic Park franchise</b>. Persistent public enthusiasm for the animals has resulted in significant funding for dinosaur science, and <b>new discoveries are regularly covered by the media</b>.</p>
      <p><u><b>This website isn't official yet, there are many changes i will do. The links for the dinosaurs wouldn't work for now.</b></u></p>
    <banner>
      <img src="dino.jpg">
    </banner>
    <h1>
      <u>Dinosaurs List</u>
    </h1>
     

   <!-- Dropdown for diet -->
    <label for="diet-filter">Choose a <b>diet</b>:</label>
    <select id="diet-filter" onchange="filterDinosaurs()">
        <option value="all">All Diets</option>
        <option value="carnivore">Carnivore</option>
        <option value="herbivore">Herbivore</option>
        <option value="omnivore">Omnivore</option>
        <option value="filter-feeder">Filter-feeder</option>
    </select>

   <!-- Dropdown for size -->
    <label for="size-filter">Choose a <b>size</b>:</label>
    <select id="size-filter" onchange="filterDinosaurs()">
        <option value="all">All Sizes</option>
        <option value="small">Small</option>
        <option value="medium">Medium</option>
        <option value="large">Large</option>
    </select>

   <!-- Dropdown for type -->
    <label for="type-filter">Choose a <b>type</b>:</label>
    <select id="type-filter" onchange="filterDinosaurs()">
        <option value="all">All Types</option>
        <option value="theropod">Theropod</option>
        <option value="sauropod">Sauropod</option>
        <option value="ornithopod">Ornithopod</option>
        <option value="ceratopsian">Ceratopsian</option>
        <option value="thyreophoran">Thyreophoran</option>
        <option value="pachycephalosaur">Pachycephalosaur</option>
        <option value="ankylosaur">Ankylosaur</option>
        <option value="pterosaur">Pterosaur</option>
        <option value="mosasaur">Mosasaur</option>
        <option value="plesiosaur">Plesiosaur</option>
        <option value="pliosaur">Pliosaur</option>
        <option value="ichthyosaur">Itchyosaur</option>
    </select>

 <!-- Dropdown for terrain -->
    <label for="terrain-filter">Choose a <b>terrain</b>:</label>
    <select id="terrain-filter" onchange="filterDinosaurs()">
        <option value="all">All Terrains</option>
        <option value="land">Land</option>
        <option value="sky">Sky</option>
        <option value="ocean">Ocean</option>
    </select>


    <!-- Dinosaur listings -->
    <div class="dinosaurs">
        <!-- Add multiple classes for each dinosaur -->
        <div class="dinosaur carnivore large theropod land">
            <a href="tyrannosaurus-rex.html" target="_blank">~T-Rex (Carnivore, Large, Theropod, Land)</a>
        </div>
       .<div class="dinosaur carnivore medium theropod land">
            <a href="velociraptor.html" targer="_blank">~Velociraptor (Carnivore, Medium, Theropod, Land)</a>
        </div>
       .<div class="dinosaur carnivore large theropod land">
            <a href="allosaurus.html" target="_blank">~Allosaurus (Carnivore, Large, Theropod, Land)</a>
        </div>
       .<div class="dinosaur carnivore large theropod land">
            <a href="spinosaurus.html" target="_blank">~Spinosaurus (Carnivore, Large, Theropod, Land)</a>
        </div>
       .<div class="dinosaur carnivore large theropod land">
            <a href="giganotosaurus.html" target="_blank">~Giganotosaurus (Carnivore, Large, Theropod, Land)</a>
        </div>
       .<div class="dinosaur carnivore large theropod land">
            <a href="carnotaurus.html" target="_blank">~Carnotaurus (Carnivore, Large, Theropod, Land)</a>
        </div>
       .<div class="dinosaur carnivore medium theropod land">
            <a href="deinonychus.html" target="_blank">~Deinonychus (Carnivore, Medium, Theropod, Land)</a>
        </div>
       .<div class="dinosaur carnivore medium theropod land">
            <a href="baryonyx.html" target="_blank">~Baryonyx (Carnivore, Medium, Theropod, Land)</a>
        </div>
       .<div class="dinosaur carnivore small theropod land">
            <a href="compsognathus.html" target="_blank">~Compsognathus (Carnivore, Small, Theropod, Land)</a>
        </div>
       .<div class="dinosaur herbivore large ceratopsian land">
            <a href="triceratops.html" target="_blank">~Triceratops (Herbivore, Large, Ceratopsian, Land)</a>
        </div>
       .<div class="dinosaur herbivore large thyreophoran land">
            <a href="stegosaurus.html" target="_blank">~Stegosaurus (Herbivore, Large, Thyreophoran, Land)</a>
        </div>
       .<div class="dinosaur herbivore large sauropod land">
            <a href="brachiosaurus.html" target="_blank">~Brachiosaurus (Herbivore, Large, Sauropod, Land)</a>
        </div>
       .<div class="dinosaur herbivore large sauropod land">
            <a href="diplodocus.html" target="_blank">~Diplodocus (Herbivore, Large, Sauropod, Land)</a>
        </div>
       .<div class="dinosaur herbivore large ankylosaur land">
            <a href="ankylosaurus.html" target="_blank">~Ankylosaurus (Herbivore, Large, Ankylosaur, Land)</a>
        </div>
       .<div class="dinosaur herbivore medium ornithopod land">
            <a href="Iguanodon.html" target="_blank">~Iguanodon (Herbivore, Medium, Ornithopod, Land)</a>
        </div>
       .<div class="dinosaur herbivore medium ornithopod land">
            <a href="parasaurolophus.html" target="_blank">~Parasaurolophus (Herbivore, Medium, Ornithopod, Land)</a>
        </div>
       .<div class="dinosaur herbivore small ornithopod land">
            <a href="hypsilophodon.html" target="_blank">~Hypsilophodon (Herbivore, Small, Ornithopod, Land)</a>
        </div>
       .<div class="dinosaur herbivore large sauropod land">
            <a href="camarasaurus.html" target="_blank">~Camarasaurus (Herbivore, Large, Sauropod, Land)</a>
        </div>
       .<div class="dinosaur herbivore medium pachycephalosaur land">
            <a href="pachycephalosaurus.html" target="_blank">~Pachycephalosaurus (Herbivore/Omnivore, Medium, Pachycephalosaur, Land)</a>
        </div>
       .<div class="dinosaur herbivore medium pachycephalosaur land">
            <a href="stygimoloch.html" target="_blank">~Stygimoloch (Herbivore/Omnivore, Medium, Pachycephalosaur, Land)</a>
        </div>
       .<div class="dinosaur herbivore medium pachycephalosaur land">
            <a href="dracorex.html" target="_blank">~Dracorex (Herbivore/Omnivore, Medium, Pachycephalosaur, Land)</a>
        </div>
       .<div class="dinosaur herbivore small pachycephalosaur land">
            <a href="stegoceras.html" target="_blank">~Stegoceras (Herbivore/Omnivore, Small, Pachycephalosaur, Land)</a>
        </div>
       .<div class="dinosaur herbivore small pachycephalosaur land">
            <a href="homalocephale.html" target="_blank">~ Homalocephale (Herbivore, Small, Pachycephalosaur, Land)</a>
        </div>
       .<div class="dinosaur herbivore medium pachycephalosaur land">
            <a href="prenocephale.html" target="_blank">~Prenocephale (Herbivore, Medium, Pachycephalosaur, Land)</a>
        </div>
       .<div class="dinosaur herbivore small pachycephalosaur land">
            <a href="goyocephale.html" target="_blank">~Goyocephale (Herbivore, Small, Pachycephalosaur, Land)</a>
        </div>
       .<div class="dinosaur herbivore large ankylosaur land">
            <a href="euoplocephalus.html" target="_blank">~Euoplocephalus (Herbivore, Large, Ankylosaur, Land)</a>
        </div>
       .<div class="dinosaur herbivore large ankylosaur land">
            <a href="saichania.html" target="_blank">~Saichania (Herbivore, Large, Ankylosaur, Land)</a>
        </div>
       .<div class="dinosaur herbivore medium ankylosaur land">
            <a href="pinacosaurus.html" target="_blank">~Pinacosaurus (Herbivore, Medium, Ankylosaur, Land)</a>
        </div>
       .<div class="dinosaur herbivore large ankylosaur land">
            <a href="tarchia.html" target="_blank">~Tarchia (Herbivore, Large, Ankylosaur, Land)</a>
        </div>
       .<div class="dinosaur herbivore small ankylosaur land">
            <a href="minmi.html" target="_blank">~Minmi (Herbivore, Small, Ankylosaur, Land)</a>
        </div>
       .<div class="dinosaur herbivore medium ankylosaur land">
            <a href="polacanthus.html" target="_blank">~Polacanthus (Herbivore, Medium, Ankylosaur, Land)</a>
        </div>
       .<div class="dinosaur herbivore medium ankylosaur land">
            <a href="nodosaurus.html" target="_blank">~Nodosaurus (Herbivore, Medium, Ankylosaur, Land)</a>
        </div>
       .<div class="dinosaur herbivore medium ankylosaur land">
            <a href="gastonia.html" target="_blank">~Gastonia (Herbivore, Medium, Ankylosaur, Land)</a>
        </div>
       .<div class="dinosaur herbivore medium ankylosaur land">
            <a href="ziapelta.html" target="_blank">~Ziapelta (Herbivore, Medium, Ankylosaur, Land)</a>
        </div>
       .<div class="dinosaur herbivore large ceratopsian land">
            <a href="styracosaurus.html" target="_blank">~Styracosaurus (Herbivore, Large, Ceratopsian, Land)</a>
        </div>
       .<div class="dinosaur herbivore large theropod land">
            <a href="therizinosaurus.html" target="_blank">~Therizinosaurus (Herbivore, Large, Theropod, Land)</a>
        </div>
       .<div class="dinosaur herbivore medium ornithopod land">
            <a href="maiasaurus.html" target="_blank">~Maiasaura (Herbivore, Medium, Ornithopod, Land)</a>
        </div>
       .<div class="dinosaur omnivore small theropod land">
            <a href="oviraptor.html" target="_blank">~Oviraptor (Omnivore, Small, Theropod, Land)</a>
        </div>
       .<div class="dinosaur omnivore small theropod land">
            <a href="troodon.html" target="_blank">~Troodon (Omnivore, Small, Theropod, Land)</a>
        </div>
       .<div class="dinosaur omnivore medium theropod land">
            <a href="gallimimus.html" target="_blank">~Gallimimus (Omnivore, Medium, Theropod, Land)</a>
        </div>
       .<div class="dinosaur omnivore medium theropod land">
            <a href="ovrnithomimus.html" target="_blank">~Ornithomimus (Omnivore, Medium, Theropod, Land)</a>
        </div>
       .<div class="dinosaur carnivore large mosasaur ocean">
            <a href="mosasaurus.html" target="_blank">~Mosasaurus (Carnivore, Large, Mosasaur, Ocean)</a>
        </div>
       .<div class="dinosaur carnivore large plesiosaur ocean">
            <a href="elasmosaurus.html" target="_blank">~Elasmosaurus (Carnivore, Large, Plesiosaur, Ocean)</a>
        </div>
       .<div class="dinosaur carnivore large pliosaur ocean">
            <a href="pliosaurus.html" target="_blank">~Pliosaurus (Carnivore, Large, Pliosaur, Ocean)</a>
        </div>
       .<div class="dinosaur carnivore large mosasaur ocean">
            <a href="tylosaurus.html" target="_blank">~Tylosaurus (Carnivore, Large, Mosasaur, Ocean)</a>
        </div>
       .<div class="dinosaur carnivore large pliosaur ocean">
            <a href="kronosaurus.html" target="_blank">~ Kronosaurus (Carnivore, Large, Pliosaur, Ocean)</a>
        </div>
       .<div class="dinosaur carnivore large pliosaur ocean">
            <a href="liopleurodon.html" target="_blank">~Liopleurodon (Carnivore, Large, Pliosaur, Ocean)</a>
        </div>
       .<div class="dinosaur carnivore medium ichthyosaur ocean">
            <a href="ichthyosaurus.html" target="_blank">~Ichthyosaurus (Carnivore, Medium, Ichthyosaur, Ocean)</a>
        </div>
       .<div class="dinosaur carnivore large ichthyosaur ocean">
            <a href="shinosaurus.html" target="_blank">~Shonisaurus (Carnivore, Large, Ichthyosaur, Ocean)</a>
        </div>
       .<div class="dinosaur carnivore medium nothosaur ocean">
            <a href="nothosaurus.html" target="_blank">~Nothosaurus (Carnivore, Medium, Nothosaur, Ocean)</a>
        </div>
       .<div class="dinosaur carnivore medium pterosaur sky land">
            <a href="pteranodon.html" target="_blank">~Pteranodon (Carnivore, Medium, Pterosaur, Sky/Land)</a>
        </div>
       .<div class="dinosaur carnivore small pterosaur sky land">
            <a href="dimorphodon.html" target="_blank">~Dimorphodon (Carnivore, Small, Pterosaur, Sky/Land)</a>
        </div>
       .<div class="dinosaur carnivore large pterosaur sky land">
            <a href="quetzalcoatlus.html" target="_blank">~Quetzalcoatlus (Carnivore, Large, Pterosaur, Sky/Land)</a>
        </div>
       .<div class="dinosaur carnivore small pterosaur sky land">
            <a href="rhamphorhynchus.html" target="_blank">~Rhamphorhynchus (Carnivore, Small, Pterosaur, Sky/Land)</a>
        </div>
       .<div class="dinosaur carnivore medium pterosaur sky land">
            <a href="tapejara.html" target="_blank">~Tapejara (Carnivore, Medium, Pterosaur, Sky/Land)</a>
        </div>
       .<div class="dinosaur carnivore medium pterosaur sky land">
            <a href="dsungaripterus.html" target="_blank">~Dsungaripterus (Carnivore, Medium, Pterosaur, Sky/Land)</a>
        </div>
       .<div class="dinosaur carnivore small pterosaur sky land">
            <a href="anurognathus.html" target="_blank">~Anurognathus (Carnivore, Small, Pterosaur, Sky/Land)</a>
        </div>
       .<div class="dinosaur filter-feeder medium pterosaur sky land">
            <a href="pterodaustro.html" target="_blank">~Pterodaustro (Filter-feeder, Medium, Pterosaur, Sky/Land)</a>
        </div>

    </div>

   <script>
        function filterDinosaurs() {
            // Get selected values from each dropdown
            const dietFilter = document.getElementById("diet-filter").value;
            const sizeFilter = document.getElementById("size-filter").value;
            const typeFilter = document.getElementById("type-filter").value;
            const terrainFilter = document.getElementById("terrain-filter").value;

            // Select all dinosaur elements
            const dinosaurs = document.querySelectorAll(".dinosaur");

            dinosaurs.forEach(dino => {
                // Check if the dinosaur matches any of the selected filters
                const matchesDiet = dietFilter === "all" || dino.classList.contains(dietFilter);
                const matchesSize = sizeFilter === "all" || dino.classList.contains(sizeFilter);
                const matchesType = typeFilter === "all" || dino.classList.contains(typeFilter);
                const matchesTerrain = terrainFilter === "all" || dino.classList.contains(terrainFilter);

                // Show the dinosaur if it matches all the filters
                if (matchesDiet && matchesSize && matchesType && matchesTerrain) {
                    dino.style.display = "block"; // Show
                } else {
                    dino.style.display = "none"; // Hide
                }
            });
        }

        // Show all dinosaurs by default on page load
        window.onload = filterDinosaurs;
    </script>
</body>
</html>
