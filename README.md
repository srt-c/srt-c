$root: '.c-rainbow';

:root {
 --color-background: #31037D;
 
 --axis-x: 1px;
 --axis-y: 1rem;
 --delay: 10;
 
 --color-black: #000;
 --color-white: #fff;
 --color-orange: #D49C3D;
 --color-red: #D14B3D;
 --color-violet: #CF52EB;
 --color-blue: #44A3F7;
 --color-green: #5ACB3C;
 --color-yellow: #DEBF40;
 
 --color-foreground: var(--color-white);
 --font-name: Righteous;
}

html, body {
 font-size: 24px;
}

body {
 background-color: var(--color-background);
 
 display: flex;
 align-items: center;
 justify-content: center;
 
 font-family: var(--font-name);
 
 height: 100vh;
}

#{$root} {
 counter-reset: rainbow;
 position: relative;
 display: block;
 
 list-style: none;
 
 padding: 0;
 margin: 0;
 
 &__layer {
  --text-color: var(--color-foreground);
  counter-increment: rainbow; 
  font-size: 3rem;
  color: var(--text-color);

  text-shadow:
   -1px -1px 0 var(--color-black),  
    1px -1px 0 var(--color-black),
    -1px 1px 0 var(--color-black),
     1px 1px 0 var(--color-black),
   
     4px 4px 0 rgba(0, 0, 0, .2);
  
  animation: rainbow 1.5s ease-in-out infinite;
  
  @for $i from 1 through 7 {
   &:nth-child(#{$i}) {
    animation-delay: calc( #{$i} / var(--delay) * 1s);
    left: calc(var(--axis-x) * #{$i});
    z-index: -#{$i * 10};
   }
  }
  
  &:not(:first-child) {
   position: absolute;
   top: 0;
  }

  &--white  { --text-color: var(--color-white)}
  &--orange { --text-color: var(--color-orange)}
  &--red    { --text-color: var(--color-red)}
  &--violet { --text-color: var(--color-violet)}
  &--blue   { --text-color: var(--color-blue)}
  &--green  { --text-color: var(--color-green)}
  &--yellow { --text-color: var(--color-yellow)}
 }
}

@keyframes rainbow {
 0%, 100% {
  transform: translatey(var(--axis-y)); 
 }
 50% {
  transform: translatey(calc(var(--axis-y) * -1));
 }
} 

<h2 align="center" font-size="bold">Hi 👋 I'm Sertac </h2>

###

<div align="center">
  <img height="150" src=""  />
</div>

###

 <p align="center">
   <a href="https://www.linkedin.com/in/sertac-kisalar">
    <img src="https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="linkedin">
  </a>
  <a href="https://codepen.io/srtcode">
    <img src="https://img.shields.io/badge/Codepen-000000?style=for-the-badge&logo=codepen&logoColor=white" alt="codepen">
  </a>
</p>

###


#  :man_technologist: About Me

- 💼 I am a Front End Developer with a background in Industrial Engineering.           
- 💬 Ask me about anything [Here](https://github.com/sertackisalar/sertackisalar/issues)
- 📫 How to reach me: [sertackisalar.me@gmail.com](mailto:sertackisalar.me@gmail.com)

###
# 💻 Tech Stack:
<div style="display: flex; justify-content: space-between;">
  <div style="flex: 1;">
    <p style="text-align: left;">
      <img src="https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white" alt="html5">
    </p>
    <p style="text-align: left;">
      <img src="https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white" alt="css3">
      <img src="https://img.shields.io/badge/SASS-hotpink.svg?style=for-the-badge&logo=SASS&logoColor=white" alt="sass">
      <img src="https://img.shields.io/badge/bootstrap-%238511FA.svg?style=for-the-badge&logo=bootstrap&logoColor=white" alt="bootstrap">
      <img src="https://img.shields.io/badge/tailwind-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white" alt="tailwind">
    </p>
    <p style="text-align: left;">
      <img src="https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E" alt="javascript">
      <img src="https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB" alt="react">
      <img src="https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white" alt="nodejs">
    </p>
    <p style="text-align: left;">
      <img src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54" alt="python">
    </p>
    <p style="text-align: left;">
      <img src="https://img.shields.io/badge/mysql-%2300000f.svg?style=for-the-badge&logo=mysql&logoColor=white" alt="mysql">
      <img src="https://img.shields.io/badge/MS%20SQL-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white" alt="microsoftsqlserver">
      <img src="https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white" alt="postgres">
      <img src="https://img.shields.io/badge/power_bi-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="powerbi">
    </p>
  </div>
  <div style="flex: 1;">
    <div style="text-align: center;">
      <img src="https://github-readme-stats.vercel.app/api?username=maurodesouza&hide_title=false&hide_rank=false&show_icons=true&include_all_commits=true&count_private=true&disable_animations=false&theme=dracula&locale=en&hide_border=false" height="150" alt="stats graph"  />
    </div>
    <div style="text-align: center;">
      <img src="https://github-readme-stats.vercel.app/api/top-langs?username=maurodesouza&locale=en&hide_title=false&layout=compact&card_width=320&langs_count=5&theme=dracula&hide_border=false" height="150" alt="languages graph"  />
    </div>
  </div>
</div>









###





