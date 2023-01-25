# Tarea-Processing_Daniel-Palacios
Tarea Processing

# https://openprocessing.org/sketch/1808817

//Daniel Palacios
// Hacer un Programa que dibuje triangulos de colores cuando se presione click
//Crear canvas
void setup() {
  size(900, 500);
}

//Definir canvas, elegir color, dibujar, y hacer un triangulo especificando los 3 vértices
void mousePressed() {
	size(900, 500);
	fill(mouseX,mouseY,mouseX/mouseY);
  stroke(255);
	triangle(mouseX, mouseY, mouseX+100, mouseY, mouseX+50, mouseY-100);
}
