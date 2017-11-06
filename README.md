int w = 80;
int h = 80;
float mappedValue;
float mappedRad; 
int multiplier = 10;




void setup() {

  size(600, 600);
}


void draw() {
  background(#D38F8F);

  mappedValue = map(mouseX,0,width,0,500);
  fill(310,50,mappedValue,30);
strokeWeight(1);
stroke(310);
  //println("mouseX: " + mouseX + "----" + "mappedValue: " + mappedValue);
  for(int i = 0; i < 10; i = i +1) {
    rect((w)*i, 0, w, h);
  }
  

    
  
  //mappedRad = map(mouseX,0,60,0,60);
  
  
  if(mappedRad > 900) {
    multiplier = -15;
    println("greater than 500");
  }
  

   if(mappedRad < 0){
    multiplier = 20;
     println("lower than 500");
  }

  
  mappedRad = mappedRad + 1 * multiplier; 
  
   ellipse(0,0,mappedRad,mappedRad);
  ellipse(100,100,mappedRad,mappedRad);
  
  
   ellipse(200,200,mappedRad,mappedRad);
   
      ellipse(300,300,mappedRad,mappedRad);
      
            ellipse(400,400,mappedRad,mappedRad);
                ellipse(500,500,mappedRad,mappedRad);
                      ellipse(600,600,mappedRad,mappedRad);
                       ellipse(700,700,mappedRad,mappedRad);
  
  
  //println(mappedRad);
  
  
  
  
  
  
  
  
}
