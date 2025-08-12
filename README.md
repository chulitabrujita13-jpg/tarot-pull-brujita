# tarot-pull-brujita{\rtf1\ansi\ansicpg1252\cocoartf2513
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\froman\fcharset0 Times-Roman;}
{\colortbl;\red255\green255\blue255;\red0\green0\blue0;}
{\*\expandedcolortbl;;\cssrgb\c0\c0\c0;}
\margl1440\margr1440\vieww10800\viewh8400\viewkind0
\deftab720
\pard\pardeftab720\partightenfactor0

\f0\fs24 \cf2 \expnd0\expndtw0\kerning0
\outl0\strokewidth0 \strokec2 <!DOCTYPE html>\
<html lang="en">\
<head>\
  <meta charset="UTF-8" />\
  <meta name="viewport" content="width=device-width, initial-scale=1" />\
  <title>Free Tarot Card Pull by Brujita</title>\
  <style>\
    body \{\
      font-family: 'Georgia', serif;\
      background: linear-gradient(135deg, #3a2c36, #6e4a7e);\
      color: #f3f0eb;\
      text-align: center;\
      padding: 50px 20px;\
      min-height: 100vh;\
      margin: 0;\
    \}\
    h1 \{\
      margin-bottom: 30px;\
      font-size: 2.5em;\
      text-shadow: 0 0 8px #bb99cc;\
    \}\
    button \{\
      background: #bb99cc;\
      border: none;\
      padding: 16px 36px;\
      font-size: 1.3em;\
      border-radius: 10px;\
      cursor: pointer;\
      color: #3a2c36;\
      font-weight: bold;\
      box-shadow: 0 0 10px #bb99cc;\
      transition: background 0.3s ease;\
    \}\
    button:hover \{\
      background: #d7bfff;\
    \}\
    .card-container \{\
      margin-top: 40px;\
      min-height: 280px;\
    \}\
    .card-name \{\
      margin-top: 15px;\
      font-style: italic;\
      font-size: 1.5em;\
      text-shadow: 0 0 5px #bb99cc;\
    \}\
    img \{\
      max-width: 220px;\
      border-radius: 12px;\
      box-shadow: 0 6px 20px rgba(187, 153, 204, 0.7);\
      user-select: none;\
    \}\
  </style>\
</head>\
<body>\
\
  <h1>Free Tarot Card Pull</h1>\
  <button onclick="drawCard()">Draw a Card</button>\
\
  <div class="card-container" id="cardContainer"></div>\
\
  <script>\
    const tarotDeck = [\
      \{\
        name: "The Fool",\
        img: "https://i.imgur.com/wF2LlB0.jpg",\
      \},\
      \{\
        name: "The Magician",\
        img: "https://i.imgur.com/OU59nmD.jpg",\
      \},\
      \{\
        name: "The High Priestess",\
        img: "https://i.imgur.com/XKM6d5Z.jpg",\
      \},\
      \{\
        name: "The Empress",\
        img: "https://i.imgur.com/mYDA5yn.jpg",\
      \},\
      \{\
        name: "The Emperor",\
        img: "https://i.imgur.com/LCXnKaG.jpg",\
      \}\
    ];\
\
    function drawCard() \{\
      const randomIndex = Math.floor(Math.random() * tarotDeck.length);\
      const card = tarotDeck[randomIndex];\
      const container = document.getElementById("cardContainer");\
      container.innerHTML = `\
        <img src="$\{card.img\}" alt="$\{card.name\}" draggable="false" />\
        <div class="card-name">$\{card.name\}</div>\
      `;\
    \}\
  </script>\
\
</body>\
</html>\
}
add tarot card pull page
