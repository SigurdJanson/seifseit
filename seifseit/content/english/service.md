---
title: "Service"
description: "this is meta description"
bg_image: "images/feature-bg.webp"
layout: "service"
draft: false
# menu:
#   main:
#     parent: "More"
#     name: "Service"
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
      icon : "icon-erlenmeyer-flask"
      color : "primary"
      content : "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Saepe enim impedit repudiandae omnis est temporibus."

    # featured service item loop
    - name : "Product Branding"
      icon : "icon-leaf"
      color : "primary-dark"
      content : "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Saepe enim impedit repudiandae omnis est temporibus."

    # featured service item loop
    - name : "Game Development"
      icon : "icon-lightbulb"
      color : "primary-darker"
      content : "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Saepe enim impedit repudiandae omnis est temporibus."



############################# Service ###############################

# These are shown on the start page 

service:
  enable : true
  title : "Principles"
  description : "... to strive for"
  service_item:
    # service item loop
    - icon : icon-infinite-outline #ionicon pack v2 : https://ionicons.com/v2/
      name: Learn 
      content: "I can tolerate failure when it helps me learn and grow. Failure without growth gnaws at me."

    # service item loop
    - icon : icon-compass-outline #ionicon pack v2 : https://ionicons.com/v2/
      name: Empower others
      content: "As a leader I am nobody without my team. It is my job to make the team strong which makes us strong."

    # service item loop
    - icon : icon-people-outline #ionicon pack v2 : https://ionicons.com/v2/
      name: Dependent Independence
      content: "Design is team work: everyone takes responsibility for each other and for themselves. There are no stars."

    # service item loop
    - icon : icon-star-half #ionicon pack v2 : https://ionicons.com/v2/
      name: Value
      content: "Incredible design drafts on paper are worth nothing unless you have the means to bring it into the product."



############################# call to action #################################
cta:
  enable : true
  # call to action content comes from "_index.md"
---
