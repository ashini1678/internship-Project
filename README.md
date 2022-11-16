![program4](https://user-images.githubusercontent.com/108610066/202230349-907d0ea7-b21c-4b73-a051-be66ad831b30.png)
![calculate-img](https://user-images.githubusercontent.com/108610066/202230362-19ebdf5c-66a9-4b12-80cd-a8ed72de0ba3.png)
![choose-img](https://user-images.githubusercontent.com/108610066/202230368-1e1f9046-3941-44ee-bec0-a2f58d21cd8a.png)
![favicon](https://user-images.githubusercontent.com/108610066/202230372-557b06e5-4b6d-4654-bc59-fa7d482420f7.png)
![home](https://user-images.githubusercontent.com/108610066/202230376-5b8c062f-d81d-4693-9c59-3b4e6e470473.jpg)
![logo1](https://user-images.githubusercontent.com/108610066/202230379-d286e05c-1f6f-4a8c-b2b3-934f8e02943c.png)
![logo2](https://user-images.githubusercontent.com/108610066/202230387-c71e8f0d-34b2-43e7-84ff-ae1cedc396c3.png)
![logo3](https://user-images.githubusercontent.com/108610066/202230396-a732bec9-d872-4403-9de0-2b532d28e456.png)
![logo4](https://user-images.githubusercontent.com/108610066/202230400-7f18ab3d-eeef-4da1-8beb-47b775e2e731.png)
![logo-nav](https://user-images.githubusercontent.com/108610066/202230408-2252b872-8f93-4663-a644-1576f75b103a.png)
![pricing1](https://user-images.githubusercontent.com/108610066/202230414-b3c35c8e-ae28-41e8-956c-4c75ee0fdd8d.png)
![pricing2](https://user-images.githubusercontent.com/108610066/202230418-1b630ed2-a4ac-4201-b1ee-6eda470681bc.png)
![pricing3](https://user-images.githubusercontent.com/108610066/202230419-15a6db60-994f-4152-801d-1ef1a43b0efb.png)
![program1](https://user-images.githubusercontent.com/108610066/202230424-207e897c-ba1f-4177-8397-82e79dc2c9e5.png)
![program2](https://user-images.githubusercontent.com/108610066/202230429-d029a586-48f2-41c7-8151-2f16d16d1c10.png)
![program3](https://user-images.githubusercontent.com/108610066/202230433-b4de2be3-b422-41ec-8032-01a9e741369f.png)
# internship-Project
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <link rel="shortcut icon" href="favicon.png" type="">
    <link href="https://cdn.jsdelivr.net/npm/remixicon@2.5.0/fonts/remixicon.css" rel="stylesheet">
    <title>Responsive Gym Website</title>


 
    
</head>

<style>

@import url("https://fonts.googleapis.com/css2?family=Kaushan+Script&family=Red+Hat+Display:wght@400;700;900&display=swap");

/*=============== VARIABLES CSS ===============*/
:root {
  --header-height: 3.5rem;

  /*========== Colors ==========*/
  /*Color mode HSL(hue, saturation, lightness)*/
  --first-color: hsl(79, 72%, 55%);
  --first-color-light: hsl(79, 97%, 77%);
  --first-color-alt: hsl(79, 67%, 52%);
  --first-color-dark: hsl(79, 63%, 50%);
  --first-color-gray: hsl(79, 6%, 64%);
  --title-color: hsl(180, 4%, 98%);
  --title-color-black: hsl(180, 4%, 12%);
  --text-color: hsl(180, 4%, 72%);
  --text-color-light: hsl(180, 4%, 65%);
  --body-color: hsl(180, 12%, 8%);

  /*========== Font and typography ==========*/
  /*.5rem = 8px | 1rem = 16px ...*/
  --body-font: 'Red Hat Display', sans-serif;
  --second-font: 'Kaushan Script', cursive;
  --biggest-font-size: 2rem;
  --bigger-font-size: 1.5rem;
  --big-font-size: 1.25rem;
  --h1-font-size: 1.5rem;
  --h2-font-size: 1.25rem;
  --h3-font-size: 1rem;
  --normal-font-size: .938rem;
  --small-font-size: .813rem;
  --smaller-font-size: .75rem;

  /*========== Font weight ==========*/
  --font-bold: 700;
  --font-black: 900;

  /*========== z index ==========*/
  --z-tooltip: 10;
  --z-fixed: 100;
}

/* Responsive typography */
@media screen and (min-width: 1024px) {
  :root {
    --biggest-font-size: 6rem;
    --bigger-font-size: 3.5rem;
    --big-font-size: 2.75rem;
    --h1-font-size: 2.25rem;
    --h2-font-size: 1.5rem;
    --h3-font-size: 1.25rem;
    --normal-font-size: 1rem;
    --small-font-size: .875rem;
    --smaller-font-size: .813rem;
  }
}

/*=============== BASE ===============*/
* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}

html {
  scroll-behavior: smooth;
}

body,
button,
input {
  font-family: var(--body-font);
  font-size: var(--normal-font-size);
}

body {
  background-color: var(--body-color);
  color: var(--text-color);
}

h1, h2, h3 {
  color: var(--title-color);
  font-weight: var(--font-bold);
}

ul {
  list-style: none;
}

a {
  text-decoration: none;
}

img {
  max-width: 100%;
  height: auto;
}

/*=============== REUSABLE CSS CLASSES ===============*/
.container {
  max-width: 1124px;
  margin-right: 1.5rem;
  margin-left: 1.5rem;
}

.section {
  padding: 4.5rem 0 2rem;
}

.section__data {
  display: flex;
  flex-direction: column;
  row-gap: .75rem;
  text-align: center;
  margin-bottom: 3rem;
}

.section__title, 
.section__title-border {
  font-size: var(--big-font-size);
  letter-spacing: 1.5px;
}

.section__subtitle {
  font-size: var(--h2-font-size);
  font-family: var(--second-font);
  font-weight: 400;
  letter-spacing: 1.5px;
  color: var(--first-color);
  transform: rotate(-2deg);
}

.section__titles {
  display: flex;
  column-gap: .75rem;
  justify-content: center;
}

.section__title-border {
  -webkit-text-stroke: 1px var(--text-color);
  color: transparent;
}

.grid {
  display: grid;
  gap: 1.5rem;
}

.main {
  overflow: hidden; /* For animation ScrollReveal */
}

.color-red {
  color: hsl(0, 80%, 64%);
}

.color-green {
  color: var(--first-color);
}

/*=============== HEADER & NAV ===============*/
.header{
    width: 100%;
    background-color: transparent;
    position: fixed;
    top: 0;
    left: 0;
    z-index: var(--z-fixed);
    transition: background .3s;

}

.nav{
    height: var(--header-height);
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.nav__logo,
.nav__toggle{
    color: var(--title-color);
    display: flex;
}

.nav__logo{
    align-items: center;
    column-gap: .5rem;
    font-weight: var(--font-bold);

}

.nav__logo img{
    width: 1.25rem;

}

.nav__toggle{
    font-size: 1.25rem;
    cursor: pointer;
}

@media  screen and (max-width: 1023px){
    .nav__menu{
        position: fixed;
        background-color: hsla(180, 12%, 8%, .8);
        backdrop-filter: blur(32px);
        -webkit-backdrop-filter: blur(32px);
        top:0;
        right: -100%;
        width: 80%;
        height: 100%;
        border-left: 2px solid var(--first-color-gray);
        transition: right .3s;
    }
}


.nav__list{
    padding: 5rem 0 0 3rem;
    display: flex;
    flex-direction: column;
    row-gap: 2.5rem;
}

.nav__link{
    color: var(--title-color);
    transition: color .3s;

}

.nav__link:hover{
    color: var(--first-color);
}

.nav__close{
    position: absolute;
    top: 1rem;
    right: 1.5rem;
    font-size: 1.5rem;
    color: var(--title-color);
    cursor: pointer; 

}

.nav .nav__button{
    background-color: var(--title-color);
    border: none;
}


/* Show menu */
.show-menu{
    right: 0;
}


/* Change background header */
.bg-header{
    background-color: var(--body-color);
    box-shadow: 0 4px 8px hsla(180, 12%, 0%, .3);
}

/* Active link */
.active-link{
color: var(--first-color);
}

/*=============== HOME ===============*/
.home{
    position: relative;
    padding-bottom: 0;
}


.home__container{
    padding-top: 4rem;
    row-gap: 3rem;
}

.home__data{
    text-align: center;
}

.home__subtitle{
    font-size: var(--bigger-font-size);
    -webkit-text-stroke: 1px var(--title-color);
    color: transparent;
}

.home__title{
    font-size: var(--bigger-font-size);
    font-weight: var(--font-black);
    margin: 5rem 0;
}

.home__subtitle,
.home__title{
    letter-spacing: 1.5px;
}

.home__description{
    margin-bottom: 2.5rem;
}

.home__triangle{
    height: 325px;
    position: absolute;
    right: 0;
    bottom: 0;
    clip-path: polygon(100% 0, 0  100%, 100% 100%);
}


.home__triangle-1{
    width: 105px;
    background-color: var(--first-color);
}
.home__triangle-2{
    width: 205px;
    background-color: var(--first-color-alt);
}
.home__triangle-3{
    width: 305px;
    background-color: var(--first-color-dark);
}

.home__img{
    display: block;
    position: relative;
    z-index: 1;
    width: 350px;
    margin: 0 auto;
}

/*=============== BUTTON ===============*/
.button{
    display: inline-block;
    background-color: var(--first-color);
    padding: 18px 32px;
    border: 2px solid var(--first-color-light);
    color: var(--title-color-black);
    font-weight: var(--font-bold);
    cursor: pointer;
    transition: background .3s;
}

.button:hover{
    background-color: var(--first-color-alt);
}

.button i{
    font-size: 1.25rem;
    transition: transform .3s;
}

.button__flex{
    display: inline-flex;
    align-items: center;
    justify-content: center;
    column-gap: .5rem;

}

.button__flex:hover i{
    transform: translateX(.25rem);
}

/*=============== LOGOS ===============*/
.logos__container{
    grid-template-columns: repeat(2, 1fr);
    gap: 2rem;
    justify-items: center;
}

.logos__img{
    width: 120px;
}


/*=============== PROGRAM ===============*/
.program__container{
    grid-template-columns: 225px;
    justify-content: center;
    row-gap: 2rem;

}

.program__card{
    display: grid;
    background-color: hsla(79 , 6%, 64%, .07);
    padding: 1.5rem 2rem;
    border: 2px solid transparent;
    transition: background .5s, border .4s;
}

.program__img{
    width: 38px;

}

.program__shape{
    width: 50px;
    height: 50px;
    background-color: var(--first-color-gray);
    border-radius: 50%;
    display: grid;
    place-items: center;
    margin-bottom: 1rem;
    transition: background .5s;
}

.program__title{
    font-size: var(--h3-font-size);
    margin-bottom: 1rem;
}

.program__description{
    font-size: var(--small-font-size);
    letter-spacing: .5px;
    line-height: 150%;
}

.program__title,
.program__description{
    transition: color .5s;
}

.program__button{
    justify-self: flex-end;
    margin-top: 1.5rem;
    font-size: 1.25rem;
    color: var(--title-color-black);
    opacity: 0;
    transition: opacity .4s;
}

.program__button i{
    display: block;
    transition: transform .3s;

}

.program__button:hover i{
    transform: translateX(.25rem);
}

.program__card:hover{
    background-color: var(--first-color);
    border: 2px solid var(--first-color-light);
}

.program__card:hover .program__shape{
    background-color: var(--first-color-light);

}

.program__card:hover .program__title,
.program__card:hover .program__description{
    color: var(--title-color-black);
}


.program__card:hover .program__button{
    opacity: 1;
}

/*=============== CHOOSE ===============*/
.choose{
    padding-bottom: 0;
}

.choose__overflow{
    position: relative
    ;

}

.choose__container{
    row-gap: 3rem;

}

.choose__content .section__data{
    margin-bottom: 2rem;
}
.choose__description{
    text-align: center;
    margin-bottom: 2.5rem;
}

.choose__data{
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    row-gap: 2rem;
}

.choose__group{
    text-align: center;
}

.choose__number{
    font-size: var(--h1-font-size);
    font-family: var(--second-font);
    font-weight: 400;
    margin-bottom: .25rem;
}

.choose__subtitle{
    font-size: var(--small-font-size);

}

.choose__triangle{
    height: 325px;
    position: absolute;
    left: 0;
    bottom: 0;
    clip-path: polygon(0 0, 0 100%, 100% 100%);
}

.choose__triangle-1{
    width: 305px;
    background-color: var(--first-color);
}
.choose__triangle-2{
    width: 205px;
    background-color: var(--first-color-alt);
}
.choose__triangle-3{
    width: 105px;
    background-color: var(--first-color-dark);
}

.choose__img{
    width: 260px;
    display: block;
    position: relative;
    z-index: 1;
    margin: 0 auto;
}

/*=============== PRICING ===============*/
.pricing__container{
    grid-template-columns: 285px;
    justify-content: center;
    row-gap: 2rem;
}

.pricing__card,
.pricing__shape,
.pricing__list{
    display: grid;
}

.pricing__card{
    row-gap: 2rem;
    background-color: hsla(79, 6%, 64%, .07);
    padding: 2rem 2.5rem;
}

.pricing__img{
    width: 35px;
}

.pricing__shape{
    width: 60px;
    height: 60px;
    background-color: var(--first-color-gray);
    border-radius: 50%;
    place-items: center;
    margin-bottom: 1rem;
}

.pricing__title{
    font-size: var(--h3-font-size);
    color: var(--text-color);
    margin-bottom: 1rem;
}

.pricing__list{
    row-gap: 1rem;

}

.pricing__item{
    display: flex;
    column-gap: .5rem;
    align-items: center;
    font-size: var(--small-font-size);
}

.pricing__item i{
    font-size: 1.25rem;
    color: var(--first-color);
}

.pricing__item-opacity{
    opacity: .3;
}


.pricing__button{
    background-color: var(--title-color);
}

.pricing__button:hover{
    background-color: var(--title-color);
}

.pricing__card-active{
    background-color: var(--first-color);
    border: 2px solid var(--first-color-light);


}

.pricing__card-active .pricing__shape{
    background-color: var(--first-color-light);
}

.pricing__card-active .pricing__item i{
    color: var(--title-color);
}

.pricing__card-active .pricing__title,
.pricing__card-active .pricing__number,
.pricing__card-active .pricing__item{
    color: var(--title-color-black);
}

/*=============== CALCULATE ===============*/
.calculate{
    padding-bottom: 0;

}

.calculate__container{
    row-gap: 4rem;
}

.calculate__content .section__titles{
    margin-bottom: 2rem;
    text-align: center;
}

.calculate__description{
    text-align: center;
    margin-bottom: 2.5rem;
}

.calculate__form{
    display: grid;
    row-gap: 1rem;
}

.calculate__box{
    position: relative;
    border: 2px solid var(--first-color-light);
}

.calculate__input{
    width: 100%;
    background: transparent;
    padding: 20px 56px 20px 24px;
    outline: none;
    border: none;
    color: var(--text-color);
}
.calculate__input::-webkit-outer-spin-button,
.calculate__input::-webkit-inner-spin-button{
    -webkit-appearance: none;

    margin: 0;
}

.calculate__input[type=number]{
    -moz-appearance: textfield;
}

.calculate__label{
    position: absolute;
    right: 1.5rem;
    top: 1.25rem;
    color: var(--title-color);
}

.calculate__form .button{
    margin-top: 1.5rem;
}

.calculate__img{
    width: 200px;
    justify-self: center;

}
.calculate__message{
    position: absolute;
    transform: translate(1rem);
}

/*=============== FOOTER ===============*/
.footer__container{
    row-gap: 4rem;
    padding-top: 1rem;
}

.footer__logo,
.footer__description{
    color: var(--title-color);
}
.footer__logo,
.footer__form,
.footer__social{
    display: flex;
}

.footer__logo{
    align-items: center;
    column-gap: .5rem;
    font-weight: var(--font-bold);
    margin-bottom: 1.5rem;
}

.footer__logo img{
    width: 1.5rem;
}

.footer__description{
    margin-bottom: 2rem;
}

.footer__form{
    flex-direction: column;
    gap: 1.25rem;
}

.footer__input{
    padding: 20px 56px 20px 24px;
    border: 2px solid var(--first-color-light);
    background: transparent;
    color: var(--text-color);
    outline: none;
}

.footer__content,
.footer__links,
.footer__group{
    display: grid;
}

.footer__content{
    grid-template-columns: repeat(2, max-content);
    gap: 2.5rem 3.5rem;
}

.footer__title{
    font-size: var(--h3-font-size);
    margin-bottom: 1.5rem;
}

.footer__links{
    row-gap: .75rem;
}

.footer__link{
    color: var(--text-color);
    transition: color .3s;
}

.footer__link:hover{
    color: var(--first-color);
}

.footer__group{
    margin-top: 5rem;
    justify-items: center;
    row-gap: 2rem;
}

.footer__social{
    column-gap: 1.25rem;
}

.footer__social-link{
    display: inline-flex;
    padding: .35rem;
    background-color: var(--first-color);
    border-radius: 50%;
    font-size: 1.25rem;
    color: var(--title-color-black);
    transition: background .4s;
}

.footer__social-link:hover{
    background-color: var(--first-color-dark);
}

.footer__copy{
    font-size: var(--smaller-font-size);
    color: var(--text-color-light);
}
.footer__message{
    position: absolute;
    transform: translateY(1rem);
}


/*=============== SCROLL BAR ===============*/
::-webkit-scrollbar{
    width: .6rem;
    border-radius: .5rem;
    background-color: hsl(79, 4%, 15%);
}

::-webkit-scrollbar-thumb{
    background-color: hsl(79, 4%, 25%);
    border-radius: .5rem;
}
::-webkit-scrollbar-thumb:hover{
    background-color: hsl(79, 4%, 35%);
    border-radius: .5rem;
}

/*=============== SCROLL UP ===============*/
.scrollup{
    position: fixed;
    right: 1rem;
    bottom: -30%;
    background-color: var(--first-color);
    display: inline-flex;
    padding: .35rem;
    color: var(--title-color-black);
    font-size: 1.25rem;
    z-index: var(--z-tooltip);
    transition: .3s;
}

.scrollup:hover{
    transform: translateY(- .25rem);
}

/* Show Scroll Up*/
.show-scroll{
    bottom: 3rem;
}

/*=============== BREAKPOINTS ===============*/
/* For small devices */
@media  screen and (max-width: 340px) {
    .container{
        margin-left: 1rem;
        margin-right: 1rem;
    }

.section__titles{
    flex-direction: column;
    row-gap: .25rem;
}

.home__triangle,
.choose__triangle{
    height: 255px;
}

.home__triangle-3,
.choose__triangle-1{
    width: 260px;
}

.choose__img{
    width: 195px;
}

.pricing__container{
    grid-template-columns: 250px;
}

.pricing__card{
    padding: 1.5rem;
}
.footer__content{
    grid-template-columns: 1fr;
}
    
}


/* For medium devices */
@media screen and (min-width: 768px){
    .nav__menu{
        width: 50%;
    }

    .home__container,
    .choose__container{
        grid-template-columns: repeat(2, 1fr);
        align-items: center;
    }
    .home__data,
    .choose__content  .section__data,
    .choose__description,
    .calculate__description{
        text-align: initial;
    }

    .logos__container{
        grid-template-columns: repeat(4, 1fr);
    }

    .program__container{
        grid-template-columns: repeat(2, 225px);
        gap: 2.5rem;
    }

    .choose__content{
        order: 1;
    }
    .choose__data{
        justify-items: flex-start;
    }
    .choose__content .section__titles,
    .calculate__content .section__titles{
        justify-content: initial;

    }

    .pricing__container{
        grid-template-columns: repeat(2, 285px);
        gap: 2.5rem;
    }

    .calculate__container{
        grid-template-columns: 1fr .8fr;
        align-items: center;
    }
    .calculate__form{
        grid-template-columns: repeat(2, 1fr);
        column-gap: 1.5rem;
    }

    .calculate__form .button{
        grid-column: 1 / 3;
    }

    .footer__container{
        grid-template-columns: repeat(2, max-content);
        justify-content: space-between;
    }

    .footer__content{
        grid-template-columns: repeat(3, max-content);
    }
}

/* For large devices */
@media screen and (min-width: 1023px) {
    

.nav{
    height: calc(var(--header-height) + 2rem);
}

.nav__menu{
    width: initial;
}

.nav__toggle,
.nav__close{
    display: none;
}

.nav__list{
    flex-direction: row;
    padding: 0;
    align-items: center;
    column-gap: 4rem;
}

.section{
    padding: 7rem 0 0;
}

.home__container{
    grid-template-columns: repeat(2, max-content);
    align-items: initial;
}

.home__title{
    margin: .75rem 0 1.25rem;
}
.home__description{
    width: 445px;
    margin-bottom: 3rem;
}
.home__img{
    width: 780px;
    transform: translateX(-6rem);
}

.home__triangle{
    height: 700px;
}
.home__triangle-1{
    width: 145px;
}
.home__triangle-2{
    width: 345px;
}
.home__triangle-3{
    width: 545px;
}

.logos{
    padding: 3.5rem 0 1rem;
}

.logos__img{
    width: 190px;
}

.choose__overflow{
    overflow: hidden;
}

.choose__img{
    width: 350px;
}

.choose__triangle{
    height: 700px;
}

.choose__triangle-1{
    width: 545px;
}
.choose__triangle-2{
    width: 345px;
}
.choose__triangle-3{
    width: 145px;
}

.footer{
    padding-bottom: 3rem;
}

.footer__form{
    flex-direction: row;
}

.footer__content{
    column-gap: 5rem;
}

.footer__group{
    grid-template-columns: repeat(2, max-content);
    justify-content: space-between;
    margin-top: 7rem;
}

.footer__social{
    order: 1;
}
}

@media screen and (min-width: 1150px) {
    .container{
        margin-left: auto;
        margin-right: auto;
    }

    .home__data{
        padding-top: 3rem;
    }

    .home__images{
        transform: translateX(-3rem);
    }

    .home__img{
        width: 800px;
        transform: translateX(2rem);
    }

    .home__triangle{
        height: 995px;
    }

    .home__triangle-1{
        width: 205px;
    }
    .home__triangle-2{
        width: 505px;
    }
    .home__triangle-3{
        width: 705px;
    }
    .program__container{
        grid-template-columns: repeat(4, 245px);
        padding: 3rem 0;
    }

    .program__card{
        padding: 2rem;
    }

    .program__description{
        font-size: var(--normal-font-size);
    }

    .choose__container{
        column-gap: 8rem;
    }
    .choose__img{
        width: 450px;
        margin: 0 0 0 auto;
    }

    .choose__triangle{
        height: 800px;
    }

    .choose__images{
        position: relative;
    }

    .choose__data{
        grid-template-columns: repeat(2, max-content);
        gap: 2.5rem 8rem;
    }

    .choose__description{
        width: 418px;
        margin-bottom: 3.5rem;
    }
    .pricing__container{
        padding-top: 3rem;
        grid-template-columns: repeat(3, 320px);
    }

    .pricing__card{
        padding: 2rem 3.5rem;
        row-gap: 2.5rem;
    }

    .calculate__description{
        width: 415px;
    }

    .calculate__form{
        width: 505px;
    }
    .calculate__img{
        width: 300px;
    }

    .scrollup{
        right: 3rem;
    }

    
}

</style>
<body>
     <!--==================== HEADER ====================-->
     <header class="header" id="header">
         <nav class="nav container">
             <a href="#" class="nav__logo">
                 <img src="logo-nav.png" alt="logo"> FITNESS MANIA
             </a>

             <div class="nav__menu" id="nav-menu">
                 <ul class="nav__list">
                     <li class="nav__item">
                         <a href="#home" class="nav__link active-link">Home</a>
                     </li>
                     <li class="nav__item">
                        <a href="#program" class="nav__link">About Us</a>
                    </li>
                    <li class="nav__item">
                        <a href="#choose" class="nav__link">Choose Us</a>
                    </li>
                    <li class="nav__item">
                        <a href="#pricing" class="nav__link">Packages</a>
                    </li>
                    <li class="nav__item">
                        <a href="#footer" class="nav__link">Contact Us</a>
                    </li>

                    <div class="nav__link">
                        <a href="#footer" class="button nav__button">
                            Register Now
                        </a>
                    </div>

                 </ul>


                 <div class="nav__close" id="nav-close">
                    <i class="ri-close-line"></i>
                 </div>
             </div>

             <div class="nav__toggle" id="nav-toggle">
                <i class="ri-menu-line"></i>
             </div>
         </nav>

    </header>

    <!--==================== MAIN ====================-->
    <main class="main">
        <!--==================== HOME ====================-->
        <section class="home section" id="home">
            <div class="home__container container grid">
                <div class="home__data">
                    <h2 class="home__subtitle">MAKE YOUR</h2>
                    <h1 class="home__title">BODY SHAPE</h1>
                    <p class="home__description">
                        In here we will help you to shape and build your ideal body and live your life to the fullest.
                    
                    </p>
                    <a href="#" class="button button__flex">
                        Get Started <i class="ri-arrow-right-line"></i>
                    </a>
                </div>

                <div class="home__images">
                    <img src="home.jpg" alt="home image" class="home__img">
                    <div class="home__triangle home__triangle-3"></div>
                    <div class="home__triangle home__triangle-2"></div>
                    <div class="home__triangle home__triangle-1"></div>
                </div>
            </div>

        </section>

        <!--==================== LOGOS ====================-->
        <section class="logos section">
            <div class="logos__container container grid">
                <img src="logo1.png" alt="logo image" class="logos__img">
                <img src="logo2.png" alt="logo image" class="logos__img">
                <img src="logo3.png" alt="logo image" class="logos__img">
                <img src="logo4.png" alt="logo image" class="logos__img">
            </div>

        </section>

        <!--==================== PROGRAM ====================-->
        <section class="program section" id="program">
            <div class="container">
                <div class="section__data">
                    <h2 class="section__subtitle">About Us</h2>
                    <div class="section__titles">
                        <h1 class="section__title-border">BUILD YOUR</h1>
                        <h1 class="section__title">BEST BODY</h1>
                    </div>
                </div>


                <div class="program__container grid">
                    <article class="program__card">
                        <div class="program__shape">
                            <img src="program1.png" alt="program image" class="program__img">
                        </div>

                        <h3 class="program__title">Flex Muscle</h3>
                        <p class="program__description">
                            Creating tension that's temporarily making the muscle fibres smaller or contracted.

                        </p>

                        <a href="#" class="program__button">
                            <i class="ri-arrow-right-line"></i>
                        </a>
                    </article>
                    <article class="program__card">
                        <div class="program__shape">
                            <img src="program2.png" alt="program image" class="program__img">
                        </div>

                        <h3 class="program__title">Cardio Exercise</h3>
                        <p class="program__description">
                            Excercise your heart rate up and keeps it up for a prolonged period of time.

                        </p>

                        <a href="#" class="program__button">
                            <i class="ri-arrow-right-line"></i>
                        </a>
                    </article>
                    <article class="program__card">
                        <div class="program__shape">
                            <img src="program3.png" alt="program image" class="program__img">
                        </div>

                        <h3 class="program__title">Basic Yoga</h3>
                        <p class="program__description">
                            Diaphgramatic this is the most common breathing teechnique you'll find in yoga.

                        </p>

                        <a href="#" class="program__button">
                            <i class="ri-arrow-right-line"></i>
                        </a>
                    </article>
                    <article class="program__card">
                        <div class="program__shape">
                            <img src="program4.png" alt="program image" class="program__img">
                        </div>

                        <h3 class="program__title">Weight Lifting</h3>
                        <p class="program__description">
                            Attempts a maximum weight single lift of a barbell loaded with weight plates.

                        </p>

                        <a href="#" class="program__button">
                            <i class="ri-arrow-right-line"></i>
                        </a>
                    </article>
                </div>
            </div>

        </section>

        <!--==================== CHOOSE US ====================-->
        <section class="choose section" id="choose">
            <div class="choose__overflow">
                <div class="choose_container container grid">
                    <div class="choose__contact">
                        <div class="section__data">
                            <h2 class="section__subtitle">Best Reason</h2>
                            <div class="section__titles">
                                <h1 class="section__title-border">WHY</h1>
                                <h1 class="section__title">CHOOSE US</h1>

                            </div>
                        </div>
                        <p class="choose_description">
                            Choose your favorite class and start now. Rememeber the only bad workout is the one you didn't do.
                        </p>
                        <div class="choose__data">
                            <div class="choose__group">
                                <h3 class="choose__number">200+</h3>
                                <p class="choose__subtitle">Total Membership</p>
                            </div>
                            <div class="choose__group">
                                <h3 class="choose__number">50+</h3>
                                <p class="choose__subtitle">Best Trainers</p>
                            </div>
                            <div class="choose__group">
                                <h3 class="choose__number">25+</h3>
                                <p class="choose__subtitle">Programs</p>
                            </div>
                            <div class="choose__group">
                                <h3 class="choose__number">100+</h3>
                                <p class="choose__subtitle">Awards</p>
                            </div>

                        </div>
                    </div>

                    <div class="choose__images">
                        <img src="choose-img.png" alt="choose image" class="choose_img">

                        <div class="choose__triangle choose__triangle-1"></div>
                        <div class="choose__triangle choose__triangle-2"></div>
                        <div class="choose__triangle choose__triangle-3"></div>
                    </div>
                </div>
            </div>

        </section>

        <!--==================== PRICING ====================-->
        <section class="pricing section" id="pricing">
            <div class="container">
                <div class="section__data">
                    <h2 class="section__subtitle">Package</h2>
                    <div class="section__titles">
                        <h1 class="section__title-border">OUR</h1>
                        <h1 class="section__title">SPECIAL PACKAGES</h1>
                    </div>
                        
                </div>

                <div class="pricing__container grid">
                    <article class="pricing__card pricing__card-active">
                        <header class="pricing__header">
                            <div class="pricing__shape">
                                <img src="pricing1.png" alt="pricing image" class="pricing__img">
                            </div>

                            <h1 class="pricing__title">BASIC PACKAGE</h1>
                            <h2 class="pricing__number">₹12000</h2>
                        </header>

                        <ul class="pricing__list">
                            <li class="pricing__item">
                                <i class="ri-checkbox-circle-line"></i> 5 Days in a week.
                            </li>
                            <li class="pricing__item">
                                <i class="ri-checkbox-circle-line"></i> 01 Sweatshirt
                            </li>
                            <li class="pricing__item pricing__item-opacity">
                                <i class="ri-checkbox-circle-line"></i> 01 Bottle of Protien
                            </li>
                            <li class="pricing__item pricing__item-opacity">
                                <i class="ri-checkbox-circle-line"></i> Access to Videos 
                            </li>
                            <li class="pricing__item pricing__item-opacity">
                                <i class="ri-checkbox-circle-line"></i> Muscle Stretching
                            </li>
                        </ul>

                        <a href="#" class="button button__flex pricing__button">
                            Purchase Now <i class="ri-arrow-right-fill"></i>
                        </a>
                    </article>
                    <article class="pricing__card">
                        <header class="pricing__header">
                            <div class="pricing__shape">
                                <img src="pricing2.png" alt="pricing image" class="pricing__img">
                            </div>

                            <h1 class="pricing__title">PREMIUM PACKAGE</h1>
                            <h2 class="pricing__number">₹25000</h2>
                        </header>

                        <ul class="pricing__list">
                            <li class="pricing__item">
                                <i class="ri-checkbox-circle-line"></i> 5 Days in a week.
                            </li>
                            <li class="pricing__item">
                                <i class="ri-checkbox-circle-line"></i> 01 Sweatshirt
                            </li>
                            <li class="pricing__item">
                                <i class="ri-checkbox-circle-line"></i> 01 Bottle of Protien
                            </li>
                            <li class="pricing__item pricing__item-opacity" >
                                <i class="ri-checkbox-circle-line"></i> Access to Videos 
                            </li>
                            <li class="pricing__item pricing__item-opacity">
                                <i class="ri-checkbox-circle-line"></i> Muscle Stretching
                            </li>
                            <li class="pricing__item pricing__item-opacity">
                                <i class="ri-checkbox-circle-line"></i> Personal Trainer
                            </li>
                        </ul>

                        <a href="#" class="button button__flex pricing__button">
                            Purchase Now <i class="ri-arrow-right-fill"></i>
                        </a>
                    </article>
                    <article class="pricing__card">
                        <header class="pricing__header">
                            <div class="pricing__shape">
                                <img src="pricing3.png" alt="pricing image" class="pricing__img">
                            </div>

                            <h1 class="pricing__title">DIAMOND PACKAGE</h1>
                            <h2 class="pricing__number">₹50000</h2>
                        </header>

                        <ul class="pricing__list">
                            <li class="pricing__item">
                                <i class="ri-checkbox-circle-line"></i> 5 Days in a week.
                            </li>
                            <li class="pricing__item">
                                <i class="ri-checkbox-circle-line"></i> 01 Sweatshirt
                            </li>
                            <li class="pricing__item">
                                <i class="ri-checkbox-circle-line"></i> 01 Bottle of Protien
                            </li>
                            <li class="pricing__item">
                                <i class="ri-checkbox-circle-line"></i> Access to Videos 
                            </li>
                            <li class="pricing__item">
                                <i class="ri-checkbox-circle-line"></i> Personal Trainer
                            </li>
                            
                        
                        </ul>

                        <a href="#" class="button button__flex pricing__button">
                            Purchase Now <i class="ri-arrow-right-fill"></i>
                        </a>
                    </article>
                    
                </div>
            </div>

        </section>
       

        <!--==================== CALCULATE ====================-->
        <section class="calculate section">
            <div class="calculate__container container grid">
                <div class="calculate__content">
                    <div class="section__titles">
                        <h1 class="section__title-border">CALCULATE</h1>
                        <h1 class="section__title">YOUR BMI</h1>
                    </div>
                    <p class="calculate__description">
                        The body mass index (BMI) calculator calculates body mass index from your weight and height.
                    </p>
                    <form action="" class="calculate__form" id="calculate-form">
                        <div class="calculate__box">
                            <input type="number" placeholder="Height" class="calculate__input" id="calculate-cm">
                            <label for="" class="calculate__label">cm</label>
                        </div>
                        <div class="calculate__box">
                            <input type="number" placeholder="Weight" class="calculate__input" id="calculate-kg">
                            <label for="" class="calculate__label">kg</label>
                        </div>
                        <button type ="submit" class="button button__flex">
                            Calculate Now <i class="ri-arrow-right-line"></i>

                        </button>
                    </form>

                    <p class="calculate__message" id="calculate-message"></p>
                </div>
                <img src="calculate-img.png" alt="calculate image" class="calculate__img">
            </div>


        </section>
    </main>

    <!--==================== FOOTER ====================-->
    <footer class="footer section" id="footer">
        <div class="footer__container container grid">
            <div>
                <a href="#" class="footer__logo">
                    <img src="logo-nav.png" alt=""> FITNESS MANIA
                </a>
                <p class="footer__description">
                    Subscribe for company <br> updates below.
                </p>
                <form action="" class="footer__form" id="contact-">
                    <input type="email" name="user_email" placeholder= "Your Email" class="footer__input" id="contact-user">
                    <button type="submit" class="button">
                        Subscribe

                    </button>
                </form>

                <p class="footer__message" id="contact-message"></p>
            </div>
            <div class="footer__content">
                <div>
                    <h3 class="footer__title">
                        SERVICES

                    </h3>
                    <ul class="footer__links">
                        <li>
                            <a href="#" class="footer link">Flex Muscle</a>
                        </li>
                        <li>
                            <a href="#" class="footer link">Cardio Excercise</a>
                        </li>
                        <li>
                            <a href="#" class="footer link">Basic Yoga</a>
                        </li>
                        <li>
                            <a href="#" class="footer link">Weight Lift</a>
                        </li>
                    </ul>
                </div>
                <div>
                    <h3 class="footer__title">
                        Packages

                    </h3>
                    <ul class="footer__links">
                        <li>
                            <a href="#" class="footer link">Basic</a>
                        </li>
                        <li>
                            <a href="#" class="footer link">Premium</a>
                        </li>
                        <li>
                            <a href="#" class="footer link">Diamond</a>
                        </li>
                    </ul>
                </div>
                <div>
                    <h3 class="footer__title">
                        COMPANY

                    </h3>
                    <ul class="footer__links">
                        <li>
                            <a href="#" class="footer link">About Us</a>
                        </li>
                        <li>
                            <a href="#" class="footer link">Careers</a>
                        </li>
                        <li>
                            <a href="#" class="footer link">Customers</a>
                        </li>
                        <li>
                            <a href="#" class="footer link">Partners</a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
        <div class="container">
            <div class="footer__group">
                <ul class="footer__social">
                    <a href="https://www.facebook.com/" target="_blank"  class="footer__social-link">
                        <i class="ri-facebook-circle-fill"></i>

                    </a>
                    <a href="https://twitter.com/" target="_blank" class="footer__social-link">
                        <i class="ri-twitter-fill"></i>
                    </a>
                    <a href="https://www.instagram.com/" target="_blank" class="footer__social-link">
                        <i class="ri-instagram-fill"></i>
                    </a>
                </ul>
                <span class="footer__copy">
                    &#169; Copyrights Bedimcode. All Rights Are Reserved.
                </span>
            </div>

        </div>

    </footer>
    <section class="pricing section" id="pricing">
        <div class="container">
            <div class="section__data">
                <h2 class="section__subtitle">Contact Us</h2>
                <div class="section__titles">
                    <h1 class="section__title">Call Us</h1>
                    <h5 class="section__title">6776898695</h5>
                    
                </div>
            </div>
    </section>

    <!--========== SCROLL UP ==========-->
    <a href="" class="scrollup" id="scroll-up">
        <i class="ri-arrow-up-line"></i>
    </a>

    <script src=""></script>
   
    <script type="text/javascript" 
    src="https://cdn.jsdelivr.net/npm/@emailjs/browser@3/dist/email.min.js">
    </script>
    
    <script>
             
    
        /*=============== SHOW MENU ===============*/
        const navMenu= document.getElementById('nav-menu'),
              navToggle = document.getElementById('nav-toggle'),
              navclose = document.getElementById('nav-close')
              
              
        if(navToggle){
            navToggle.addEventListener('click',() =>{
                navMenu.classList.add('show-menu')
            })
        }
        
        
        if(navclose){
            navclose.addEventListener('click', () =>{
                navMenu.classList.remove('show-menu')
            })
        }
        
        const navLink =  document.querySelectorAll('.nav__link')
        const linkAction = () =>{
            const navMenu = document.getElementById('nav-menu')
            navMenu.classList.remove('show-menu')
        
        
        }
        
        navLink.forEach(n => n.addEventListener('click', linkAction))
        
        const scrollHeader = () =>{
            const header = document.getElementById('header')
            this.scrollY >= 50 ? header.classList.add('bg-header')
                                : header.classList.remove('bg-header')
        } 
        
        window.addEventListener('scroll' , scrollHeader);
        
        
        
         
        /*=============== REMOVE MENU MOBILE ===============*/
        
        
        /*=============== CHANGE BACKGROUND HEADER ===============*/
        
        
        /*=============== SCROLL SECTIONS ACTIVE LINK ===============*/
        const sections = document.querySelectorAll('section[id]')
    
        const scrollActive = () =>{
            const scrollY = window.pageYOffset
    
            sections.forEach(current =>{
                const sectionHeight = current.offsetHeight
                sectionTop = current.offsetTop -58
                sectionId = current.getAttribute('id')
                sectionsClass = document.querySelector('.nav__menu a[href*=' + sectionId + ']')
            if(scrollY > sectionTop && scrollY <= sectionTop + sectionHeight){
                sectionsClass.classList.add('active-link')
            }else{
                sectionsClass.classList.remove('active-link')
            }
    
            })
        }
    window.addEventListener('scroll', scrollActive)
        /*=============== SHOW SCROLL UP ===============*/ 
    const scrollUp = () =>{
        const scrollUp = document.getElementById('scroll-up')
        this.scrollY >= 350? scrollUp.classList.add('show-scroll')
                                                : scrollUp.classList.remove('show-scroll')
    }
    window.addEventListener('scroll', scrollUp)
        
        /*=============== SCROLL REVEAL ANIMATION ===============*/
        const sr= ScrollReveal({
            origin: 'top',
            distance: '60px',
            duration: 2500,
            delay: 400,
    
        })
    
        sr.reveal('.home__data')
        sr.reveal('.home__img', {delay: 700, origin: 'bottom'})
        sr.reveal('.logos__img', {interval: 100})
        
        /*=============== CALCULATE JS ===============*/
        const calculateForm = document.getElementById('calculate-form')
              calculateCm = document.getElementById('calculate-cm')
              calculateKg = document.getElementById('calculate-kg')
              calculateMessage = document.getElementById('calculate-message')
        
        const calculateBmi = (e) =>{
            e.preventDefault()
        
            if(calculateCm.value === '' || calculateKg.value === ''){
                calculateMessage.classList.remove('color-green')
                calculateMessage.classList.add('color-red')
        
                calculateMessage.textContent = 'Fill in the Height and Weight 🏋️‍♀️'
                setTimeout(() =>{
                    calculateMessage.textContent = ''
                }, 3000)
        
            } else{
                const cm = calculateCm.value / 100
                      kg= calculateKg.value
                      bmi = Math.round(kg / (cm *cm))
        
                if(bmi < 18.5){
                    calculateMessage.classList.add('color-green')
                    calculateMessage.textContent= 'You are skinny'
                
                } else if(bmi<25){
                    calculateMessage.classList.add('color-green')
                    calculateMessage.textContent= 'You are healthy'
                }
                else{
                    calculateMessage.classList.add('color-green')
                    calculateMessage.textContent= 'You are overweight'
                }
        
                calculateCm.value = ''
                calculateKg.value = ''
        
                setTimeout(() =>{
                    calculateMessage.textContent = ''
                }, 4000)
            }
        }
        
        calculateForm.addEventListener('submit', calculateBmi)
        
        
        
            
        
        
        /*=============== EMAIL JS ===============*/
    
    
        const contactForm = document.getElementById('contact-form')
              contactMessage = document.getElementById('contact-message')
              contactUser = document.getElementById('contact-user')
        
        const sendEmail = (e) =>{
            e.preventDefault()
        
            if(contactUser.value === ''){
            contactMessage.classList.remove('color-green')
            contactMessage.classList.add('color-green')
        
            contactMessage.textContent = 'You must enter your Email'
        
            setTimeout(() =>{
                contactMessage.textContent = ''
            }, 3000)
        } else{
            emailjs.sendForm('service_s6aokc9','template_9v9qodp','#contact-form','BL43eY3EyCgaMrUGC')
            .then(()=> {
                contactMessage.classList.add('color-green')
                contactMessage.textContent = 'You registered sucessfully 💪'
    
                setTimeout(()=>{
                    contactMessage.textContent=''
                }, 3000)
            },(error) =>{
                alert('OOPS! SOMETHING HAS FAILED...', error)
            })
    
            contactUser.value=''
        }
        }
        
        contactForm.addEventListener('submit' , sendEmail)
        
       
    
    
        
    </script>

   
</body>
</html>
