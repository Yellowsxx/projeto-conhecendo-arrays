let circuloX = [];
let circuloY = [];
let cor;

function setup() {
  createCanvas(400, 400);
  background(100, 0, 0);
  circuloX = [0, 0, 0];
  circuloY = [random(height), random(height), random(height)];
  cor = color(random(0, 255), random(0, 255), random(0, 255));
}

function draw() {
  fill(cor);
  for (let contador = 0; contador < circuloX.length; contador++) {
    circle(circuloX[contador], circuloY[contador], 50);
    circuloX[contador] += random(0, 3);
    circuloY[contador] += random(-3, 3);
    if (circuloX[contador] >= width) {
      circuloX[contador] = 0;
      circuloY[contador] = random(height);
    }
  }
  if (mouseIsPressed) {
    cor = color(random(0, 255), random(0, 255), random(0, 255), random(0, 100));
  }
}
