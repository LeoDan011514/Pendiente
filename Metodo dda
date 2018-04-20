let m=0
let b=0
let x=0
let y=0
let k=0
let steps=0
let dx
let dy
let xIncremento
let yIncremento

function setup() {
	createCanvas(windowWidth,windowHeight);
}

function draw()
{
	pintar(0,0,windowWidth,windowHeight)
	pintar(0,windowHeight,windowWidth,0)
	pintar(0,windowHeight/2,windowWidth,windowHeight/2)
	pintar(windowWidth/2,0,windowWidth/2,windowHeight)
}

function pintar(x1,y1,x2,y2){

	m = (y2-y1)/(x2-x1)
	x = x1
	y = y1
	steps = x2-x1 // pasos
	// delta x 
	dx = x2 - x1;
	dy = y2 - y1;
	x = x1; 
	y = y1;

	//valor absoluto solo para ver la diferencia entre las diferencias
	// si no pones abs y estan de derecha a izq como debe dibujar
	// no lo va dibujar por que la diferencia de uno es negativa por lo cual lo hace menor y/o affecta de donde a donde debe dibujar
	if (abs(dx) > abs(dy)){
		steps = dx;
	}else{
		steps = dy;
	}
	// si |dy| > 1 entonces dy/steps el cual es igual a dy  da 1 entonces
	// la y se va ir sumando en 1 y la x parcialmente por que queda dx/dif el cual 
	// representa 1/m
	// en casos de dx siendo mayor que 1 se incrementara en 1 y dy en algo parcial

	xIncremento= dx/steps;
	yIncremento = dy/steps;

	point (x,y);
	for (let k = 0; k < steps; k++)
	{
		x += xIncremento;
		y += yIncremento;
	point (x,y);
	}
}
