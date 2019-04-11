## What is StellarICO.Expert?

It is the best way to document or promote your Stellar ICO, Stellar Security Token Offer (STO), Stellar Utility Token, Stellar Equity Tokens, Airdrop, and or Bounty program if exists already or is in the planning phase. For users it is the easiest way to keep on top of upcoming or past projects that they are interested in or finding new ones. 

While many other ico promotion sites charge for listings - Stellar ICO Expert is free. Stellar ICO Expert data is 100% driven by the community via github so all submissions and changes can be easily merged into our high performance static website. While on other sites your stellar token event may get overwhelmed by Ethereum coins. All data is creative commons and can be used by other websites. This means that for stellar people update just one website instead of dozens when dates or values change.
To get listed you need to only follow two criteria. First it must use the stellar blockchain and second it must follow the stellar community guidelines https://www.stellar.org/community-guidelines/.

The second goal of the project is to come up with machine readable format for ICOs in toml, yaml, json, or xml format. To see your listing 24-48 hours after submitted visit https://stellarico.expert and any other sites supporting this format.

Ratings for the icos are done on completeness of data.

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
   - No spaces in names please and use unix format   

## images size 
    logo 150x150 px
    banner 800x300 px 
    screenshot 350x200 px


   - title : < title/name of the ico> String
  - date : 2018-11-08 00:00:00
    - when ico is created in iso date format
  - tags : ["upcoming","Payments","airdrop"]
    - add tags here (Array of strings)
  - categories : ["upcoming", "Payments","airdrop"]
    - add categories it must contain one of these ( "active", "upcoming",  "ended" ) otherwise ico will not display on home page (List of strings)
  - ticket : "Payments"
    - String
  - banner : "img/ico/tempo/background.jpg"
    - banner path (string) do not include 'static/'
    - String
  - logo : "img/ico/tempo/Tempo_logo_white150x150.jpg"
    - ico logo path (string) do not include 'static/'
  - description : "The easiest, fastest and most secure bridge between cash and crypto!"
    - Add short description (string 150 chars)
  - long_description:
        "<h5>Blah blah blah....Neque porro quisquam est qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit Neque porro quisquam est qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit Neque porro quisquam est qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit</h5>"
     - Add long description (Mardown)
 - start_date: 2018-11-08 00:00:00
   - start of ico (including presale in iso date format)
 - end_date : 2018-11-18 00:00:00Z
   - end of ico (including presale in iso date format)
 - rating : 3
  - will be automatically generated
 - ticker : TEMPO
 - token_type : STELLAR
 - token_price: "1 TEMPO = 0.1200 EUR"
 - funds_raise_todate: 1000000 integer
 - funds_softcap_goal : 1500000 integer
 - funds_hardcap_goal: 7000000 integer
 - available_for_token_sale: 20%
  - this is the percent of tokens available for sale
 - kyc: YES (1 JAN - AUG – 7 SEP)
 - accepted_currency :  BTC, ETH, XRP, XLM, EURT, EUR, JPY
 - non_participate: NORTH KOREA, CUBA, Syria, Crimea/Sevastopol, USA (limited)
 - airdrop : YES
  - String or (in case boolean put it within single quotes)
  - If you do not include it will not appear
 - airdrop_live : NO
   - if not airdrop is available please do not include these fields
 - country: FR
    - ISO2 of the country
 - bounty : "https://ico.tempo.eu.com/bounty"
    - URL
    - If you do not include it will not appear
   - a URL to a page or website that describes the bounty process
   - if there is no bounty this field should not appear or be empty
 - additional_links : ["https://sharespost.com/",
        "https://glassnet.io/downloads/GLASS_Executive_Summary.pdf",
        "https://glassnet.io/blog/"]
    - array of string URL
 - screenshots :
            [ "/img/ico/blockcloud/screenshots/1.jpg",
              "/img/ico/blockcloud/screenshots/2.jpg",
              "/img/ico/blockcloud/screenshots/3.jpg",
              "/img/ico/blockcloud/screenshots/4.jpg",]
   - array of string (screenshot path)
 - website : "https://ico.tempo.eu.com"
   - URL
 - whitepaper_url : "https://irp-cdn.multiscreensite.com/d3d3962e/files/uploaded/TEMPO-Whitepaper-pre-release-v27.a.pdf.pdf"
   - URL
 - twitter_url : "https://twitter.com/tempo_eu"
   - URL
 - telegram_url : "https://t.me/joinchat/Cl6wihECcZFcv2tJcFEY5Q"
   - URL
 - github_url: ""
   - URL
 - reddit_url: ""
   - URL
 - facebook_url: ""
   - URL
 - og_png: "img/ico/blockcloud/Blockcloud-Main.jpg"
   - URL
 - tw_png: "img/ico/blockcloud/Blockcloud-Main.jpg"
   - URL
- stellarport_url : ""
   - if this is an exisiting asset, go to stellarport.io, click on exchange, assets and search for the ticker.
   - url required if ended and Stellar ICO otherwise do not include
  - stellarx_url : ""
   - if this is an exisiting asset, go to stellarx.com, click on market and search for the ticker.
   - url required if ended and Stellar ICO and is listed on stellarx otherwise do not include
 - stellarexpert_url : ""
    - go to stellar.expert and add the url to the asset
    - type the ticker into the search box
    - url required if ended and Stellar ICO
  - coinmarketcap_url : ""
    - if asset has coinmarketcap listing add here
    - should be URL
 - weight: 5
   - give the weight to ICO 0 (zero is minimun ) on the basis of this weight ico will show on home page


  Push any changes and they will automatically be accepted once reviewed and pushed to the website. 



