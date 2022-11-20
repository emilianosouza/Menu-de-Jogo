# Menu-de-Jogo


var tela = 1;
var largura = 200;
var altura = 50;
var xMenu = 50;
var yMenu1 = 50;
var yMenu2 = 115;
var yMenu3 = 180

function setup() {
  createCanvas(300, 300);
}

function draw() {
  textStyle(NORMAL)

//TELA DE MENU
  
//BOTAO INICIO
  if (tela == 1){
    background(20,50,100)
    textAlign(CENTER);
    textSize(26);
  
  if (mouseX > xMenu && mouseX < xMenu + largura && mouseY > yMenu1 && mouseY < yMenu1 + altura){
    stroke(300)
    fill(20)
    rect(xMenu, yMenu1, largura, altura, 15) 
  if (mouseIsPressed){
      tela = 2
    
  }
 }
}
    fill(300)
    noStroke()
    text(" Iniciar", 150, 85)

  
  
//BOTÃO CREDITOS
  if (mouseX > xMenu && mouseX < xMenu + largura && mouseY > yMenu2 && mouseY < yMenu2 + altura){
    stroke(300)
    fill(20)
    rect(xMenu, yMenu2, largura, altura, 15) 
  if (mouseIsPressed){
      tela = 3
  }
}
  
    fill(300)
    noStroke()
    text(" Créditos", 150, 145)
  
//BOTÃO INSTRUÇÃO
  if (mouseX > xMenu && mouseX < xMenu + largura && mouseY > yMenu3 && mouseY < yMenu3 + altura){
    stroke(300)
    fill(20)
    rect(50,yMenu3, largura, altura, 15)
  if (mouseIsPressed){
      tela = 4
  }
}

    fill(300)
    noStroke()
    text(" Instruções", 150, 210)
}
  






  
  


