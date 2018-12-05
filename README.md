## What is StellarICO.Expert?

It is the best way to promote your Stellar ICO, Stellar Token, Stellar Utility Token, Stellar Equity Token, Airdrop, and or Bounty program if exists already or is in the planning phase. For users it is the easiest way to keep on top of upcoming or past projects that they are interested in or finding new ones. 

While many other ico promotion sites charge for listings - Stellar ICO Expert is free. Stellar ICO Expert data is 100% driven by the community via github so all submissions and changes can be easily merged into our high performance static website. While on other sites your stellar token event may get overwhelmed by Ethereum s** coins.

To get listed you need to only follow two criteria. First it must use the stellar blockchain and second it must follow the stellar community guidelines https://www.stellar.org/community-guidelines/.

The second goal of the project is to come up with machine readable format for ICOs in toml, yaml, json, or xml format.nTo see your listing 24-48 hours after submitted visit https://stellarico.expert

# How do you get started? 

First it helps if you know a bit about git. Read these items first if you don't

https://github.com/WGBH/pbucore/wiki/Contributing-to-the-project-through-Github-web-interface
and you would fork the repo and then request pull
to create folders you need to create the file or upload it
https://stackoverflow.com/questions/18773598/creating-folders-inside-github-com-repo-without-using-git

or

https://akrabat.com/the-beginners-guide-to-contributing-to-a-github-project/

ALL files should use unix forward slashes when refering to images.

## Getting Started

Clone :

    git clone https://github.com/antb123/stellarico.git \
    && cd stellarico \


## How to add a new ico
  1. Go to content folder
  
   - copy an existing ico and paste in the same folder 
   - rename it with new ico name that you want to submit 
    
    e.g : cp content/ico/tempocrypto.md content/ico/<new_iconame>.md
    mkdir /static/img/ico/<new_iconame>
    mkdir /static/img/ico/<new_iconame>/screenshots
    
  2. update the variables.
  
  [**Variables**](#variables)
  
  3. Add images
   - logo : /static/img/ico/<new_iconame>/logo.png 
   - banner : /static/img/ico/<new_iconame>/banner.png 
   - screenshots : 
     - Screenshots should be of important images from an app or the whitepaper
     - /static/img/ico/tempocrypto/<new_iconame>/screenshots/1.png
     - /static/img/ico/tempocrypto/<new_iconame>/screenshots/2.png
     - /static/img/ico/tempocrypto/<new_iconame>/screenshots/3.png
     

## images size 
    logo 150x150 px
    banner 800x300 px 
    screenshot 350x200 px


## variables

  - title : < title/name of the ico>
  - date : "2018-11-08T00:00:00Z"
    - when ico is created
  - tags : ["upcoming","Payments","airdrop"] 
    - add tags here are upcoming, ended, active
    - active is for icos currenty occuring, whereas upcoming are in the future and ended are complete
    - the next tag is the type - you can copy this from another site in terms of category
    - the final tag is if there is an airdrop or not. If there is no airdrop remove this tag
  - categories : ["upcoming", "Payments","airdrop"]
    - add categories it must contain one of these ( "active", "upcoming",   "ended" ) otherwise ico will not display on home page
    - again the other two follow the tags
  - ticket : "Payments"
     - this should be the type
  - banner : "img/ico/tempocrpto/background.jpg"
    - banner path
  - logo : "img/ico/tempo/Tempo_logo_white150x150.jpg"
    - logo path
  - image : ""
    -this is optional  
  - description : "The easiest, fastest and most secure bridge between cash and crypto!"
  - long_description: "Blah blah blah....Neque porro quisquam est qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit Neque porro quisquam est qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit Neque porro quisquam est qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit"
 - money_goal : "1,000,000" 
 - goal : "7,000,000 (13%)"
 - start_date: "2018-11-08T00:00:00Z"
 - end_date : "2018-11-18T00:00:00Z"
 - rating : 
   - this is filled in automatically based on social proof. For Tokens that are live it comes from a 50/50 mixture of stellar.expert and stellarport ratings.
 - ticker : TEMPO
 - token_type : STELLAR
 - token_price: "1 TEMPO = 0.1200 EUR"
 - softcap_goal: 1,500,000 EUR
 - fundraising_goal: 7,000,000 EUR
 - available_for_token_sale: 20%
 - kyc: YES (1 JAN - AUG – 7 SEP)
 - accepted_currency :  BTC, ETH, XRP, XLM, EURT, EUR, JPY
 - non_participate: NORTH KOREA, CUBA, Syria, Crimea/Sevastopol, USA (limited)
 - airdrop : YES
 - airdrop_live : NO
   - if there is no airdrop do not include these two variables and they will not appear
 - country: FR
 - bounty : "https://ico.tempo.eu.com/bounty"
 - additional_links : ["https://stellar.org/",
        "https://tempo.eu.com/"] 
 - screenshots : 
            [ "/img/ico/tempocrypto/screenshots/1.jpg",
              "/img/ico/tempocrypto/screenshots/2.jpg",
              "/img/ico/tempocrypto/screenshots/3.jpg",
              "/img/ico/tempocrypto/screenshots/4.jpg",] 
   - screenshot path
 - website : "https://ico.tempo.eu.com"
 - whitepaper_url : "https://irp-cdn.multiscreensite.com/d3d3962e/files/uploaded/TEMPO-Whitepaper-pre-release-v27.a.pdf.pdf"
 - twitter_url : "https://twitter.com/tempo_eu"
 - telegram_url : "https://t.me/joinchat/Cl6wihECcZFcv2tJcFEY5Q"
 - github_url: "https://github.com/tempofr"
 - reddit_url: "https://www.reddit.com/user/TempoMoneyTransfer"
 - facebook_url: "https://www.facebook.com/TEMPOMoneyTransfer/"
 - bitcointalk_url : "https://bitcointalk.org/index.php?topic=5025231.msg45455624#msg45455624"
 - youtube_url : "https://www.youtube.com/channel/UC-MI1jnOA1T1ublc6QoJ71w"
 - linkedin_url : "https://fr.linkedin.com/company/tempo-france-sas"
   - all these social sites are optional. If they are not included they will not appear on your page
  - stellarport_url : ""
   - if this is and exisiting asset, go to stellarport.io, click on exchange, assets and search for the ticker.
   if it exists add the url
 - stellarexpert_url : ""
    - go to stellar.expert and add the url to the asset 
    - type the ticker into the search box
 - og_png: "img/ico/tempocrypto/Tempo-Main.jpg"
 - tw_png: "img/ico/tempocrypto/Tempo-Main.jpg"
 - weight: 5 
   - give the weight to ICO 0 (zero is minimum ) on the basis of this weight ico will show on home page 
   
  Push any changes and they will automatically be accepted once reviewed and pushed to the website. 



