---
############################### Banner ##############################
banner:
  enable: true
  bg_image: "images/illustration.png"
  bg_overlay: true
  title: "The Office"
  content: "We love the office and through the conducted analysis we are trying to make you love it as well"
  button:
    enable: true
    label: "Our Goal"
    link: "goal"

############################# About #################################
about:
  enable: true
  title: "To explore The Office, we use several datasets:"
  content: " 
    - We first extract all the characters that played in the Office from season 1 to season 9 (final). This is extracted using [*Dunderpedia: The Office Wiki*](https://theoffice.fandom.com/)
    
    - A description of each character is downloaded from the same source: [*Dunderpedia: The Office Wiki*](https://theoffice.fandom.com/). This data is used to extract the sentiment of each character and will later be compared to the sentiment extracted from the episodes transcripts. We would like to validate that the character description is based on the character developemnt over all seasons. 
    
    
    - We then want to analyse episodes ratings The Office and how they change overtime. We use the [*IMDB*](https://www.imdb.com/title/tt0386676/episodes/_ajax)  to extract: episode title, [*IMDB*](https://www.imdb.com/title/tt0386676/episodes/_ajax) rating, total votes ad air date.
    
    
    - From [*Kaggle data*](https://www.kaggle.com/andreal314159/the-office-analysis-for-datacamp/data) we download the guest starts, directors adn writers. We use this data to analyse the impact of guest starts, directors and writers in the ratings. 
    
    
    - Next, to further analyse the episodes raitings, we want to get information about the episode itself, such as the characters that played in it, how many lines they had in every episode and so on. This is collected from a [*Kaggle dataset*](https://www.kaggle.com/nasirkhalid24/the-office-us-complete-dialoguetranscript/version/1?select=The-Office-Lines.csv): *The Office (US) - Complete Dialogue/Transcript*
  "
  image: "images/michael_explain.gif"
  services:
  - HTML5 Markup
  


######################### Portfolio ###############################
portfolio:
  enable: true
  bg_image: "images/office.png"
  title: "Want to see more?"
  content: ""
  button:
    enable: true
    label: "View Data"
    link: "https://github.com/saralopez7/theOffice-socialGraphs-analysis/tree/master/data"


############################# Service ############################
service:
  enable: true
  # service content comes from "service.md" file


############################ call to action ###########################
cta:
  enable: true
  bg_image: "images/call-to-action-bg.jpg"
  title: "We got you covered"
  content: "See the full code and data"
  button:
    enable: true
    label: "Notebook"
    link: "https://wetransfer.com/downloads/45a28a7ad7f76459d4a9993e9c83198220211206122833/cbe07e"

############################# Funfacts ###############################
funfacts:
  enable: true
  title: "Fun Facts About Us"
  description: "'Not all of us have watched The Office'"
  funfact_item:
  # funfacts item loop
  - icon: "fas fa-mug-hot" #https://fontawesome.com/v5.15/icons
    name: "Cups Of Coffee"
    count: "99"

  # funfacts item loop
  - icon: "fas fa-glasses" #https://fontawesome.com/v5.15/icons
    name: "Article Written"
    count: "45"

  # funfacts item loop
  - icon: "fas fa-keyboard" #https://fontawesome.com/v5.15/icons
    name: "Goals Completed"
    count: "125"

  # funfacts item loop
  - icon: "fas fa-clock" #https://fontawesome.com/v5.15/icons
    name: "Hours spent"
    count: "210"

  testimonial_slider:
  # testimonial item loop
  - name: "Michael Scott"
    image: "images/testimonial_m.jpg"
    designation: "Branch Manager"
    content: "And I knew exactly what to do. But in a much more real sense, I had no idea what to do."

  # testimonial item loop
  - name: "Dwight Schrute"
    image: "images/testimonials2.jpg"
    designation: "Assistant to the regional Manager"
    content: "If I were buying my coffin, I would get one with thicker walls so you couldn’t hear the other dead people."

  # testimonial item loop
  - name: "Kelly Kapoor"
    image: "images/kelly.jpg"
    designation: "Customer Service"
    content: "I am one of those few people who looks hot eating a cupcake."


---
