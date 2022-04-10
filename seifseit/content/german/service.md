---
title: "Dienstleistungen"
description: "this is meta description"
bg_image: "images/feature-bg.jpg"
layout: "service"
draft: false
# menu:
#   main:
#     parent: "Mehr"
#     name: "Dienstleistung"
#     weight: 1


########################### about service #############################
about:
  enable : false
  title : "Creative UX/UI Design Agency"
  content : "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptate soluta corporis odit, optio
          cum! Accusantium numquam ab, natus excepturi architecto earum ipsa aliquam, illum, omnis rerum, eveniet
          officia nihil. Eum quod iure nulla, soluta architecto distinctio. Nesciunt odio ullam expedita, neque fugit
          maiores sunt perferendis placeat autem animi, nihil quis suscipit quibusdam ut reiciendis doloribus natus nemo
          id quod illum aut culpa perspiciatis consequuntur tempore? Facilis nam vitae iure quisquam eius harum
          consequatur sapiente assumenda, officia voluptas quas numquam placeat, alias molestias nisi laudantium
          nesciunt perspiciatis suscipit hic voluptate corporis id distinctio earum. Dolor reprehenderit fuga dolore
          officia adipisci neque!"
  image : "images/company/company-group-pic.jpg"


########################## featured service ############################
featured_service:
  enable : false
  service_item:
    # featured service item loop
    - name : "Interface Design"
      icon : "ion-erlenmeyer-flask"
      color : "primary"
      content : "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Saepe enim impedit repudiandae omnis est temporibus."

    # featured service item loop
    - name : "Product Branding"
      icon : "ion-leaf"
      color : "primary-dark"
      content : "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Saepe enim impedit repudiandae omnis est temporibus."

    # featured service item loop
    - name : "Game Development"
      icon : "ion-lightbulb"
      color : "primary-darker"
      content : "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Saepe enim impedit repudiandae omnis est temporibus."



############################# Service ###############################

# These are shown on the start page 

service:
  enable : true
  title : "Prinzipien"
  description : "... für die sich der Einsatz lohnt"
  service_item:
    # service item loop
    - icon : ion-ios-infinite #ionicon pack v2 : https://ionicons.com/v2/
      name: Lernen
      content: "Ich komme klar, wenn mal etwas schief geht. Daraus lerne ich. Kann ich das nicht, machts mich verrückt."

    # service item loop
    - icon : ion-compass #ionicon pack v2 : https://ionicons.com/v2/
      name: Andere stark machen
      content: "Der Design Leader ist nichts ohne ein Team. Mach ich das Team stark, mach ich uns alle stark."

    # service item loop
    - icon : ion-ios-people-outline #ionicon pack v2 : https://ionicons.com/v2/
      name: Abhängig unabhängig
      content: "Design ist Teamarbeit: jeder muss Verantwortung für den anderen übernehmen und sich selbst. Es gibt keinen Star."

    # service item loop
    - icon : ion-android-star-half #ionicon pack v2 : https://ionicons.com/v2/
      name: Werthaltig
      content: "Das atemberaubendste Design auf Papier ist völlig wertlos, wenn Ihr nicht die Mittel habt, das ins Produkt zu bringen."



############################# call to action #################################
cta:
  enable : true
  # call to action content comes from "_index.md"
---
