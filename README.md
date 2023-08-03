- 👋 Hi, I’m @Germaryori
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
int nX = 55;
int nY=55;
int lives = 5;
void setup () { 
  size (600,600); 
 background (0);

}
void draw (){
background(0);
 stroke(0,0,255);
 strokeWeight(10);
 line(30,50,30,150);
 line(80,50,80,100);
  line(80,100,500,100);
  line (30,150,450,150);
  line (500,100,500,250);
  line(450,150,450,200);
  line(450,200,30,200);
  line(500,250,80,250);
  line(30,200,30,400);
  line(80,250,80,350);
  line(30,400,450,400);
  line(80,350,500,350);
  line(450,400,450,470);
  line(500,350,500,470);
  noStroke();
  fill(0,255,0);
 ellipse(nX,nY,30,30);
  
  if( nX < 50){
  nX= 55 ;
   nY =55;  
    lives = lives -1; 
  }
     if ( nX > 480 ) {
       nX=55;
       nY =55; 
       lives = lives -1; 
       
     }
     if((nX > 60) && (nY < 120)) { 
       nX=55;
       nY = 55;
       lives = lives -1; 
     }
     if ((nX < 460 )&& (nY > 380)) {
       nX = 55;
       nY =55;
       lives = lives -1; 
 }
 if(( nX < 470)&& ( nY > 130 )&& (nY < 220)){
        nX = 55;
       nY =55;
   lives = lives -1; 
 }
 if (( nX > 60) && (nY > 230) && ( nY < 370)){
          nX = 55;
       nY =55;
   lives = lives -1; 
 }
                   
  text("lives = "+lives,width-80,10);            
  if (lives<=0)                                  
  {
    textSize(50);
    text("Game Over ", 150,300);   
     noLoop(); 
    lost=true;
    textSize(50);
  }
  if ( nX >=500 , nY >= 500 )
  { 
        textSize(50);
    text(" WINNER ", 150,300);
    noLoop();                                   
    lost=true;
    textSize(50);
  }
 }
    void keyPressed() {
  if (keyCode == RIGHT) {
    nX = nX + 6;
  }

  if (keyCode == LEFT) {
   nX = nX - 6;
}
 if (keyCode == UP){
   nY=nY -6;
 }
 if (keyCode== DOWN){
   nY=nY +6 ; 
 }
    }
<!---
Germaryori/Germaryori is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
