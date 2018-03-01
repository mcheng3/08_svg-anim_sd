var pic = document.getElementById("pic");
var hasMadeFirst = false;
var x_0 = 0;
var y_0 = 0;

var drawCircle = function(e){
    x = e.offsetX;
    y = e.offsetY;
    if(!hasMadeFirst) hasMadeFirst = true;
	else drawLine(x, y);

    var c = document.createElementNS( "http://www.w3.org/2000/svg","circle");
	c.setAttribute("cx", x);
	c.setAttribute("cy", y);
	c.setAttribute("r", "10");
	c.setAttribute("fill", "lightsteelblue");
	pic.appendChild(c);

	x_0 = x
	y_0 = y
};

var drawLine = function(x2, y2){
	var l = document.createElementNS( "http://www.w3.org/2000/svg","line");
	l.setAttribute("x1", x_0);
	l.setAttribute("y1", y_0);
	l.setAttribute("x2", x);
	l.setAttribute("y2", y);
	l.setAttribute("stroke", "black");
	l.setAttribute("fill", "black");
	console.log(l);
	pic.appendChild(l);
};

var clear = function(){
	pic.innerHTML = "";
	hasMadeFirst = false;
};

pic.addEventListener("click", drawCircle);
document.getElementById("clear").addEventListener("click", clear);