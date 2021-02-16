<! DOCTYPE html >
< html  lang = " it " >
  < testa >
    < script  src = " https://cdnjs.cloudflare.com/ajax/libs/p5.js/1.1.9/p5.js " > </ script >
    < meta  charset = " utf-8 " />
    < stile >
    html ,  body {
      margine : 0 ;
      imbottitura : 0 ;
    }
    tela {
      display : blocco;
    }
    </ style >
    < title > Chicken Robot </ title >
  </ head >
  < corpo >
  < script >
  function  setup ( )  {
  createCanvas ( 400 ,  400 ) ;
}

funzione  draw ( )  {
sfondo ( "ciano" ) ;

  riempimento ( "bianco" ) ;
  noStroke ( )
  arco ( 40 , 100 , 35 , 35 , PI , TWO_PI ) ;
  arco ( 65 , 100 , 45 , 45 , PI , TWO_PI ) ;
  arco ( 90 , 100 , 35 , 35 , PI , TWO_PI ) ;

  arco ( 140 , 80 , 35 , 35 , PI , TWO_PI ) ;
  arco ( 165 , 80 , 45 , 45 , PI , TWO_PI ) ;
  arco ( 190 , 80 , 35 , 35 , PI , TWO_PI ) ;

  arco ( 190 , 120 , 35 , 35 , PI , TWO_PI ) ;
  arco ( 215 , 120 , 45 , 45 , PI , TWO_PI ) ;
  arco ( 240 , 120 , 35 , 35 , PI , TWO_PI ) ;

  arco ( 315 , 90 , 35 , 35 , PI , TWO_PI ) ;
  arco ( 340 , 90 , 45 , 45 , PI , TWO_PI ) ;
  arco ( 365 , 90 , 35 , 35 , PI , TWO_PI ) ;
  // nuvole
  riempimento ( "verde" )
  rect ( 0 , 350 , 400 , 350 ) ;

    corsa ( 1 )
  linea ( 200 , 0 , 200 , 400 ) ;
  // linea di simmetria
  riempimento ( 128 , 0 , 128 ) ;
  cerchio ( mouseX - 0 , mouseY - 0 , 70 ) ;
  riempimento ( 227 , 11 , 92 ) ;
  cerchio ( mouseX - 0 , mouseY - 0 , 50 ) ;
  // testa
  riempimento ( 128 , 0 , 128 ) ;
  cerchio ( mouseX + 20 , mouseY - 0 , 10 ) ;
  cerchio ( mouseX - 20 , mouseY - 0 , 10 ) ;
  // occhi
  linea ( mouseX - 39 , mouseY - 55,5 , mouseX - 17,5 , mouseY - 31 ) ;
  cerchio ( mouseX - 39 , mouseY - 55,5 , 8 ) ;
  linea ( mouseX + 39 , mouseY - 55,5 , mouseX + 17,5 , mouseY - 31 ) ;
  cerchio ( mouseX + 39 , mouseY - 55,5 , 8 ) ;
  // antenne
  arco ( mouseX - 35 , mouseY - 0 , 10 , 10 , HALF_PI , 4.8 , OPEN ) ;
  arco ( mouseX + 35 , mouseY + 0 , 10 , 10 , 4.8 , HALF_PI , OPEN ) ;
  // orecchie
  triangolo ( mouseX + 0 , mouseY + 0 , mouseX - 10 , mouseY + 5 , mouseX + 10 , mouseY + 5 ) ;
  // becco
  rect ( mouseX - 10 , mouseY + 35 , 20 , 10 ) ;
  // collo
  riempimento ( 128 , 0 , 128 ) ;
  rect ( mouseX - 40 , mouseY + 40 , 80 , 75 , 15 ) ;
  riempimento ( 227 , 11 , 92 ) ;
  rect ( mouseX - 25 , mouseY + 52,5 , 50 , 50 , 15 ) ;
  // parte superiore del corpo
  quadrato ( mouseX - 55 , mouseY + 50 , 15 , 5 ) ;
  quadrato ( mouseX + 40,5 , mouseY + 50 , 15 , 5 ) ;
  riempimento ( 49 , 0 , 98 ) ;
  rect ( mouseX - 63 , mouseY + 50 , 8.5 , 15 ) ;
  riempimento ( 210 , 105 , 30 ) ;
  arco ( mouseX - 63,5 , mouseY + 57,5 , 15 , 15 , HALF_PI , 4.80 ) ;
  riempimento ( 49 , 0 , 98 ) ;
  rect ( mouseX + 55 , mouseY + 50 , 8.5 , 15 ) ;
  riempimento ( 210 , 105 , 30 ) ;
  arco ( mouseX + 63,5 , mouseY + 57,5 , 15 , 15 , 4.80 , HALF_PI ) ;
  // spalle
  riempimento ( 227 , 11 , 92 ) ;
  rect ( mouseX - 63 , mouseY + 66 , 10 , 60 ) ;
  riempimento ( 49 , 0 , 98 ) ;
  cerchio ( mouseX - 58 , mouseY + 100 , 15 ) ;
  arco ( mouseX - 58 , mouseY + 125 , 10 , 10 , TWO_PI , PI ) ;
  riempimento ( 227 , 11 , 92 ) ;
  rect ( mouseX - 60.5 , mouseY + 130 , 5 , 7 )
  riempimento ( 218 , 186 , 208 ) ;
  arco ( mouseX - 58 , mouseY + 137 , 20 , 20 , TWO_PI , PI , CHORD )
  // braccio destro
  riempimento ( 227 , 11 , 92 ) ;
  rect ( mouseX + 53 , mouseY + 65 , 10 , 60 ) ;
  riempimento ( 49 , 0 , 98 ) ;
  cerchio ( mouseX + 58 , mouseY + 100 , 15 ) ;
  arco ( mouseX + 58 , mouseY + 125 , 10 , 10 , TWO_PI , PI ) ;
  riempimento ( 257 , 11 , 92 ) ;
  rect ( mouseX + 55,5 , mouseY + 130 , 5 , 7 ) ;
  riempimento ( 218 , 186 , 208 ) ;
  arco ( mouseX + 58 , mouseY + 137 , 20 , 20 , TWO_PI , PI , CHORD ) ;
  // braccio sinistro
  riempimento ( 227 , 11 , 92 ) ;
  rect ( mouseX - 20 , mouseY + 115 , 10 , 60 ) ;
  riempimento ( 49 , 0 , 98 ) ;
  cerchio ( mouseX - 15 , mouseY + 145 , 15 )
  riempimento ( 218 , 186 , 208 ) ;
  arco ( mouseX - 15 , mouseY + 175 , 20 , 20 , PI , TWO_PI , CHORD ) ;
  // gamba destra
  riempimento ( 227 , 11 , 92 ) ;
  rect ( mouseX + 10 , mouseY + 115 , 10 , 60 ) ;
  riempimento ( 49 , 0 , 98 ) ;
  cerchio ( mouseX + 15 , mouseY + 145 , 15 ) ;
  riempimento ( 218 , 186 , 208 ) ;
  arco ( mouseX + 15 , mouseY + 175 , 20 , 20 , PI , TWO_PI , CHORD ) ;
  // gamba sinistra
  }
  </ script >
  </ body >
</ html ># integramento.github.io
a
