# Tarea-Processing_Daniel-Palacios
Tarea Processing



boolean newletter;              

int numChars = 26;      // There are 26 characters in the alphabet
color[] colors = new color[numChars];

void setup() {
  size(640, 360);
  colorMode(HSB, width, height, 100); 
  noStroke();
}


void draw() {
  int whichBar = mouseX / barWidth;
  if (whichBar != lastBar) {
    int barX = whichBar * barWidth;
    fill(barX, mouseY, 66);
    rect(barX, 0, barWidth, height);
    lastBar = whichBar;
  }
}
