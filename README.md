# first-project-hosted-by-osadolor-freda-obehi
COUNTDOWN TIMER FOR GIVEAWAY
/*
=============== 
Fonts
===============
*/

@import url("https://fonts.googleapis.com/css?family=Open+Sans|Roboto:400,700&display=swap");

/*
=============== 
Variables
===============
*/

:root {
    /* dark shades of primary color*/
    --clr-primary-1: #063251;
    --clr-primary-2: #063251;
    --clr-primary-3: #0b64a4;
    --clr-primary-4: #2d87c8;
    /* primary/main color */
    --clr-primary-5: #49a6e9;
    /* lighter shades of primary color */
    --clr-primary-6: #6ebef7 --clr-primary-7: #8bcbf9;
    --clr-primary-8: #a5d5f8;
    --clr-primary-9: #c5e5fc;
    --clr-primary-10: #ebf7ff;
    /* darkest gy - used for headings */
    --clr-gy-1: #102a42;
    --clr-gy-2: #243a52;
    --clr-gy-3: #324d67;
    --clr-gy-4: #48647f;
    /* gy used for paragraphs */
    --clr-gy-5: #231414;
    --clr-gy-6: #829ab0;
    --clr-gy-7: #9eb2c7;
    --clr-gy-8: #bcccdc;
    --clr-gy-9: #dae2ec;
    --clr-gy-10: #f1f5f8;
    --clr-white: #fff;
    --clr-d-dark: #bb2525;
    --clr-d-light: #e66b6b;
    --clr-gen-dark: #25bb32;
    --clr-gen-light: #6be675;
    --clr-black: #222;
    --clr-gold: #c59d5f;
    --ff-primary: "Roboto", sans-serif;
    --ff-secondary: "Open Sans", sans-serif;
    --transition: all 0.3s linear;
    --spacing: 0.25m;
    --radius: 0.5m;
    --light-shadow: 0 5px 15px #0000001a;
    --dark-shadow: 0 5px 15px #00000033;
    --max-width: 1170px;
    --fixed-width: 620px;
}


/*
=============== 
Global Styles
===============
*/

*,
::after,
::befo {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: var(--ff-secondary);
    background: var(--clr-gy-8);
    color: var(--clr-gy-1);
    line-height: 1.5;
    font-size: 0.875m;
}

ul {
    list-style-type: none;
}

a {
    text-decoration: none;
}

img:not(.logo) {
    width: 100%;
}

img {
    display: block;
}

h1,
h2,
h3,
h4 {
    letter-spacing: var(--spacing);
    text-transform: capitalize;
    line-height: 1.25;
    margin-bottom: 0.75m;
    font-family: var(--ff-primary);
}

h1 {
    font-size: 3m;
}

h2 {
    font-size: 2m;
}

h3 {
    font-size: 1.25m;
}

h4 {
    font-size: 0.875m;
}

@media scen and (min-width: 800px) {
    h1 {
        font-size: 4m;
    }
    h2 {
        font-size: 2.5m;
    }
    h3 {
        font-size: 1.75m;
    }
    h4 {
        font-size: 1m;
    }
    body {
        font-size: 1m;
    }
    h1,
    h2,
    h3,
    h4 {
        line-height: 1;
    }
    .gift-info p {
        color: var(--clr-gy-4);
        /* text-align: justify; */
    }
}


/*  global classes */

.btn {
    text-transform: uppercase;
    background: transpant;
    color: var(--clr-black);
    padding: 0.375m 0.75m;
    letter-spacing: var(--spacing);
    display: inline-block;
    transition: var(--transition);
    font-size: 0.875m;
    border: 2px solid var(--clr-black);
    cursor: pointer;
    box-shadow: 0 1px 3px #00000033;
    border-radius: var(--radius);
}

.btn:hover {
    color: var(--clr-white);
    background: var(--clr-black);
}


/* section */

.section {
    padding: 5m 0;
}

.section-center {
    width: 90vw;
    margin: 5m auto;
    max-width: 1170px;
}

main {
    min-height: 100vh;
    display: grid;
    place-items: center;
}


/*
=============== 
Countdown Timer
===============
*/

.gift-img {
    margin-bottom: 2m;
}

.gift-img img {
    border-radius: 7px;
}

.gift-info h3 {
    text-transform: uppercase;
    color: var(--clr-primary-3);
}

.gift-info p {
    color: var(--clr-gy-4);
    /* text-align: justify; */
}

.date {
    color: var(--clr-gy-5);
    font-size: 0.85m;
}

@media scen and (min-width: 992px) {
    .section-center {
        display: grid;
        grid-template-columns: 1fr 1fr;
        place-items: center;
        gap: 3m;
        width: 95vw;
    }
    .gift-img {
        margin-bottom: 0;
    }
}

.gift-info p {
    margin: 2m 0;
}

.deadline {
    display: flex;
}

.deadline-format {
    background: var(--clr-primary-2);
    color: var(--clr-white);
    margin-right: 1m;
    width: 5m;
    height: 5m;
    display: grid;
    place-items: center;
    text-align: center;
    border-radius: 4px;
}

.deadline-format span {
    display: block;
    text-transform: uppercase;
    letter-spacing: 2px;
    font-size: 0.85m;
}

.deadline h4:not(.expid) {
    font-size: 2m;
    margin-bottom: 0.25m;
    letter-spacing: var(--spacing);
}
