---
############################### Banner ##############################
banner:
  enable: true
  bg_image: "images/illustration.png"
  bg_overlay: true
  title: "The Office"
  content: "Click the below button for an in depth analysis of The Office tv show!"
  button:
    enable: true
    label: "View Analysis"
    link: "blog"

############################# About #################################
about:
  enable: true
  title: "To explore The Office, we use several datasets:"
  content: " 
  ### Dunderpedia: The Office Wiki.
  
  #### Encyclopedia dedicated to housing an informative database for all subject matter related to The Office.

- Using [**Dunderpedia: The Office Wiki**](https://theoffice.fandom.com/) we first extracted all the characters that played in The Office from season 1 to season 9 (final). Besides, we downloaded the description of each character.     
This data was used to create a network between all of the characters of The Office based on their descriptions.  To achieve this goal we have used regular expressions! From the network, we identified communities. Moreover, we used the character descriptions to create word-clouds for 16 of the main characters. 

#### IMDb 
IMDb Ratings of The Office

- Using [**IMDb**](https://www.imdb.com/title/tt0386676) we extracted information about every episode of every season of The Office. This includes episode titles for all seasons, IMDb ratings, total votes, description and air date of every episode. 

This data was used for exploratory data analysis of the popularity and success of The Office throughout the seasons. More specifically, on its own, this dataset was used to study the variation of votes, views and ratings during the 9 seasons and perform analysis for what went wrong in seasons 8 and 9 after Michael (the main character) left. Then it was combined with the Transcripts dataset to analyse the impact of every character on the success of the show.

#### Kaggle: The Office Dataset
Dataset of all episodes of the popular US TV Series - The Office

 - From [**Kaggle**](https://www.kaggle.com/nehaprabhavalkar/the-office-dataset), we downloaded The Office dataset to extend the previously downloaded IMDb data. The new data includes guest stars, directors and writers. 
 
  It is important to note that even though this Office dataset from Kaggle also contains the ratings and Viewership of the Office, it has not been updated since `September 2020`. Therefore, we wanted to extract these data directly from IMDb to have the most up-to-date ratings and views. Since The Office is still available on Network and has been watched 50.1 billion times in 2020, these ratings are likely to be changing frequently. Hence, from this Kaggle dataset, we only took the static data: guest stars, writers and directors. 
 This data was used to analyse the impact of guest stars, directors and writers on the ratings and views. We analysed the most talented writers and directors and the ratings when episodes were directed or written by members of the cast. Then we looked into the best director-writer combinations with respect to ratings.
 
 
####  Kaggle: The Office (US) - Complete Dialogue/Transcript
45,000+ lines of dialogue from 9 seasons of The Office

 - To further analyse the episode ratings, we needed information about the episode itself, such as the cast for each episode and the lines for each character in every episode. This is collected from the [**Kaggle dataset: The Office (US) - Complete Dialogue/Transcript**](https://www.kaggle.com/nasirkhalid24/the-office-us-complete-dialoguetranscript/version/1?select=The-Office-Lines.csv)."
  image: "images/michael_explain.gif"



######################### Portfolio ###############################
# portfolio:
#   enable: true
#   bg_image: "images/office.png"
#   title: "Want to see more?"
#   content: ""
#   button:
#     enable: true
#     label: "View Data"
#     link: "https://github.com/saralopez7/theOffice-socialGraphs-analysis/tree/master/data"


############################# Service ############################
service:
  enable: true
  # service content comes from "service.md" file


############################ call to action ###########################
cta:
  enable: true
  bg_image: "images/theofficepicture.PNG"
  title: "We got you covered"
  content: "See the full code and data"
  button:
    enable: true
    label: "Repository"
    link: "https://github.com/saralopez7/theOffice-socialGraphs-analysis"

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
    count: "12"

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
    image: "images/michael.png"
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
