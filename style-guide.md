@import url('https://fonts.googleapis.com/css2?family=Fraunces:opsz,wght@9..144,100;9..144,200;9..144,300;9..144,400;9..144,500;9..144,600;9..144,700;9..144,800;9..144,900&family=Montserrat:wght@100;200;300;400;500;600;700;800;900&display=swap');

@font-face {
  font-family: 'Montserrat';
  src: url('fonts/Montserrat.ttf');

  font-family: 'Fraunces';
  src: url('fonts/Fraunces.ttf');
}

body {
  background-color: hsl(30, 38%, 92%);
  font-family: 'Fraunces', sans-serif;
  overflow-x: hidden;
}

p {
  font-size: 14px;
  font-family: 'Montserrat';
  font-weight: 500;
}

h1 {
  margin-top: -5px;
  font-weight: 700;
}

.container {
  display: grid;
  margin: 1.7em auto;
  width: 95%;
  border-radius: 5px;
  background-color: white;
}

.container .mobileImg {
  display: block;
  margin: auto;
  width: 100%;
  border-radius: 10px 10px 0 0;
}

.desktopImg {
  display: none;
}

.description {
  margin: .5em auto;
  width: 90%;
}

.description span {
  letter-spacing: 4px;
  font-weight: 500;
  color: gray;
}

.description p {
  font-weight: 500;
  letter-spacing: 1px;
  font-size: .74em;
  line-height: 1.75;
  color: gray;
}

.description h2 {
  color: hsl(158, 36%, 37%);
}

.description strike {
  position: absolute;
  font-size: .5em;
  font-family: 'Montserrat';
  font-weight: 500;
  color: gray;
  padding-left: 20px;
  margin-top: 7px;
}

button:hover {
  background-color: #1a4031;
}

button {
  display: inline-flex;
  padding: 0;
  margin: 0 auto;
  margin-bottom: 15px;
  width: 300px;
  height: 45px;
  background-color: hsl(158, 36%, 37%);
  font-family: 'Montserrat';
  font-weight: 700;
  border-radius: 10px;
  border-style: none;
  font-size: 1em;
}

.buttonIcon{
  display: inline-flex;
  align-items: center;
  padding: 13px 40px;
  color: white;
  position: absolute;
  padding-left: 100px;
}

button p {
  margin: 0 auto;
  padding-left: 30px;
  padding-top: 13px;
  color: white !important;
}

@media all and (min-width: 1366px) {

  .container {
    display: inherit;
    margin-top: 130px;
    display: grid;
    width: 40%;
    height: 30%;
    justify-content: center;
    border-radius: 10px;
  }

  .container .mobileImg {
    display: none;
  }

  .container .desktopImg {
    display: block;
    width: 50%;
    height: auto;
    padding-right: 8px;
    border-radius: 10px 0 0 10px;
  }

  .container .description {
    position: absolute;
    margin-left: 335px;
    margin-top: 20px;
    width: 16%;
  }

  .description p {
    width: 95%;
  }

  .description h2 {
    font-size: 30px;
  }

  .description button {
    width: 240px;
    height: 50px;
  }

  .buttonIcon{
    padding-top: 15px;
    padding-left: 60px;
  }

  button p {
    padding-top: 13px;
    padding-left: 35px;
    font-size: 0.9em !important;
  }
}