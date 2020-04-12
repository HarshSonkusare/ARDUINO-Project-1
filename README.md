int red1=13,yellow1=12,green1=11, red2=10,yellow2=9,green2=8,red3=7,yellow3=6,green3=5,red4=4,yellow4=3,green4=2;

void setup()

{

pinMode(red1, OUTPUT);
pinMode(yellow1, OUTPUT);
pinMode(green1, OUTPUT);  

  pinMode(red2, OUTPUT);
pinMode(yellow2, OUTPUT);
pinMode(green2, OUTPUT);  

  pinMode(red3, OUTPUT);
pinMode(yellow3, OUTPUT);
pinMode(green3, OUTPUT);  

  pinMode(red4, OUTPUT);
pinMode(yellow4, OUTPUT);
pinMode(green4, OUTPUT);  

Serial.begin(9600);

while (!Serial);

Serial.println("Input 1 or 2 or 3 or 4");

}

void loop() {

if (Serial.available())

{

int time_slot = Serial.parseInt();

if (time_slot == 1)

{
for(int i=1;i>0;i++)
{
digitalWrite(red1,LOW); digitalWrite(yellow1,HIGH); digitalWrite(green1,LOW);
digitalWrite(red2,LOW); digitalWrite(yellow2,HIGH); digitalWrite(green2,LOW);
digitalWrite(red3,LOW); digitalWrite(yellow3,HIGH); digitalWrite(green3,LOW);
digitalWrite(red4,LOW); digitalWrite(yellow4,HIGH); digitalWrite(green4,LOW);
  delay(1000);
digitalWrite(red1,LOW); digitalWrite(yellow1,LOW); digitalWrite(green1,LOW);
digitalWrite(red2,LOW); digitalWrite(yellow2,LOW); digitalWrite(green2,LOW);
digitalWrite(red3,LOW); digitalWrite(yellow3,LOW); digitalWrite(green3,LOW);
digitalWrite(red4,LOW); digitalWrite(yellow4,LOW); digitalWrite(green4,LOW);
  delay(1000);
}
}

if (time_slot == 2)

{
for(int i=1;i>0;i++)
{

  if(i%4 == 1)
  { digitalWrite(red1,LOW); digitalWrite(yellow1,LOW); digitalWrite(green1,HIGH);
	digitalWrite(red2,HIGH); digitalWrite(yellow2,LOW); digitalWrite(green2,LOW);
	digitalWrite(red3,HIGH); digitalWrite(yellow3,LOW); digitalWrite(green3,LOW);
	digitalWrite(red4,HIGH); digitalWrite(yellow4,LOW); digitalWrite(green4,LOW);
  	delay(3000);
    digitalWrite(red1,LOW); digitalWrite(yellow1,HIGH); digitalWrite(green1,LOW);
	digitalWrite(red2,HIGH); digitalWrite(yellow2,LOW); digitalWrite(green2,LOW);
	digitalWrite(red3,HIGH); digitalWrite(yellow3,LOW); digitalWrite(green3,LOW);
	digitalWrite(red4,HIGH); digitalWrite(yellow4,LOW); digitalWrite(green4,LOW);
    delay(1000);}
                                          
    
  if(i%4 == 2)
    {
    digitalWrite(red1,HIGH); digitalWrite(yellow1,LOW); digitalWrite(green1,LOW);
	digitalWrite(red2,LOW); digitalWrite(yellow2,LOW); digitalWrite(green2,HIGH);	
	digitalWrite(red3,HIGH); digitalWrite(yellow3,LOW); digitalWrite(green3,LOW);
	digitalWrite(red4,HIGH); digitalWrite(yellow4,LOW); digitalWrite(green4,LOW);
    delay(3000);
    digitalWrite(red1,HIGH); digitalWrite(yellow1,LOW); digitalWrite(green1,LOW);
	digitalWrite(red2,LOW); digitalWrite(yellow2,HIGH); digitalWrite(green2,LOW);
	digitalWrite(red3,HIGH); digitalWrite(yellow3,LOW); digitalWrite(green3,LOW);
	digitalWrite(red4,HIGH); digitalWrite(yellow4,LOW); digitalWrite(green4,LOW);
    delay(1000);
    }
                        
  if(i%4 == 3)
    {
    digitalWrite(red1,HIGH); digitalWrite(yellow1,LOW); digitalWrite(green1,LOW);
	digitalWrite(red2,HIGH); digitalWrite(yellow2,LOW); digitalWrite(green2,LOW);	
	digitalWrite(red3,LOW); digitalWrite(yellow3,LOW); digitalWrite(green3,HIGH);
	digitalWrite(red4,HIGH); digitalWrite(yellow4,LOW); digitalWrite(green4,LOW);
    delay(3000);
    digitalWrite(red1,HIGH); digitalWrite(yellow1,LOW); digitalWrite(green1,LOW);
	digitalWrite(red2,HIGH); digitalWrite(yellow2,LOW); digitalWrite(green2,LOW);
	digitalWrite(red3,LOW); digitalWrite(yellow3,HIGH); digitalWrite(green3,LOW);
	digitalWrite(red4,HIGH); digitalWrite(yellow4,LOW); digitalWrite(green4,LOW);
    delay(1000);
    }
                                         
  if(i%4 == 0)
    {
    digitalWrite(red1,HIGH); digitalWrite(yellow1,LOW); digitalWrite(green1,LOW);
	digitalWrite(red2,HIGH); digitalWrite(yellow2,LOW); digitalWrite(green2,LOW);	
	digitalWrite(red3,HIGH); digitalWrite(yellow3,LOW); digitalWrite(green3,LOW);
	digitalWrite(red4,LOW); digitalWrite(yellow4,LOW); digitalWrite(green4,HIGH);
    delay(3000);
    digitalWrite(red1,HIGH); digitalWrite(yellow1,LOW); digitalWrite(green1,LOW);
	digitalWrite(red2,HIGH); digitalWrite(yellow2,LOW); digitalWrite(green2,LOW);
	digitalWrite(red3,HIGH); digitalWrite(yellow3,LOW); digitalWrite(green3,LOW);
	digitalWrite(red4,LOW); digitalWrite(yellow4,HIGH); digitalWrite(green4,LOW);
    delay(1000);
    }
}
}
  
if (time_slot == 3)

{
for(int i=1;i>0;i++)
{
  
  if(i%2 == 1)
    {digitalWrite(red1,HIGH); digitalWrite(yellow1,LOW); digitalWrite(green1,LOW);
	 digitalWrite(red2,LOW); digitalWrite(yellow2,LOW); digitalWrite(green2,HIGH);
	 digitalWrite(red3,HIGH); digitalWrite(yellow3,LOW); digitalWrite(green3,LOW);
	 digitalWrite(red4,LOW); digitalWrite(yellow4,LOW); digitalWrite(green4,HIGH);
     delay(3000);
     digitalWrite(red1,HIGH); digitalWrite(yellow1,LOW); digitalWrite(green1,LOW);
	 digitalWrite(red2,LOW); digitalWrite(yellow2,HIGH); digitalWrite(green2,LOW);
	 digitalWrite(red3,HIGH); digitalWrite(yellow3,LOW); digitalWrite(green3,LOW);
	 digitalWrite(red4,LOW); digitalWrite(yellow4,HIGH); digitalWrite(green4,LOW);
     delay(1000);}
                                          
  if(i%2 == 0)
    {digitalWrite(red1,LOW); digitalWrite(yellow1,LOW); digitalWrite(green1,HIGH);
	 digitalWrite(red2,HIGH); digitalWrite(yellow2,LOW); digitalWrite(green2,LOW);
	 digitalWrite(red3,LOW); digitalWrite(yellow3,LOW); digitalWrite(green3,HIGH);
	 digitalWrite(red4,HIGH); digitalWrite(yellow4,LOW); digitalWrite(green4,LOW);
     delay(3000);
     digitalWrite(red1,LOW); digitalWrite(yellow1,HIGH); digitalWrite(green1,LOW);
	 digitalWrite(red2,HIGH); digitalWrite(yellow2,LOW); digitalWrite(green2,LOW);
	 digitalWrite(red3,LOW); digitalWrite(yellow3,HIGH); digitalWrite(green3,LOW);
	 digitalWrite(red4,HIGH); digitalWrite(yellow4,LOW); digitalWrite(green4,LOW);
     delay(1000);}
}
}

if (time_slot == 4)
for(int i=1;i>0;i++)
{

  if(i%4 == 1)
  { digitalWrite(red1,LOW); digitalWrite(yellow1,LOW); digitalWrite(green1,HIGH);
	digitalWrite(red2,HIGH); digitalWrite(yellow2,LOW); digitalWrite(green2,LOW);
	digitalWrite(red3,HIGH); digitalWrite(yellow3,LOW); digitalWrite(green3,LOW);
	digitalWrite(red4,HIGH); digitalWrite(yellow4,LOW); digitalWrite(green4,LOW);
  	delay(3000);
    digitalWrite(red1,LOW); digitalWrite(yellow1,HIGH); digitalWrite(green1,LOW);
	digitalWrite(red2,HIGH); digitalWrite(yellow2,LOW); digitalWrite(green2,LOW);
	digitalWrite(red3,HIGH); digitalWrite(yellow3,LOW); digitalWrite(green3,LOW);
	digitalWrite(red4,HIGH); digitalWrite(yellow4,LOW); digitalWrite(green4,LOW);
    delay(1000);}
                                          
    
  if(i%4 == 2)
    {
    digitalWrite(red1,HIGH); digitalWrite(yellow1,LOW); digitalWrite(green1,LOW);
	digitalWrite(red2,LOW); digitalWrite(yellow2,LOW); digitalWrite(green2,HIGH);	
	digitalWrite(red3,HIGH); digitalWrite(yellow3,LOW); digitalWrite(green3,LOW);
	digitalWrite(red4,HIGH); digitalWrite(yellow4,LOW); digitalWrite(green4,LOW);
    delay(3000);
    digitalWrite(red1,HIGH); digitalWrite(yellow1,LOW); digitalWrite(green1,LOW);
	digitalWrite(red2,LOW); digitalWrite(yellow2,HIGH); digitalWrite(green2,LOW);
	digitalWrite(red3,HIGH); digitalWrite(yellow3,LOW); digitalWrite(green3,LOW);
	digitalWrite(red4,HIGH); digitalWrite(yellow4,LOW); digitalWrite(green4,LOW);
    delay(1000);
    }
                        
  if(i%4 == 3)
    {
    digitalWrite(red1,HIGH); digitalWrite(yellow1,LOW); digitalWrite(green1,LOW);
	digitalWrite(red2,HIGH); digitalWrite(yellow2,LOW); digitalWrite(green2,LOW);	
	digitalWrite(red3,LOW); digitalWrite(yellow3,LOW); digitalWrite(green3,HIGH);
	digitalWrite(red4,HIGH); digitalWrite(yellow4,LOW); digitalWrite(green4,LOW);
    delay(3000);
    digitalWrite(red1,HIGH); digitalWrite(yellow1,LOW); digitalWrite(green1,LOW);
	digitalWrite(red2,HIGH); digitalWrite(yellow2,LOW); digitalWrite(green2,LOW);
	digitalWrite(red3,LOW); digitalWrite(yellow3,HIGH); digitalWrite(green3,LOW);
	digitalWrite(red4,HIGH); digitalWrite(yellow4,LOW); digitalWrite(green4,LOW);
    delay(1000);
    }
                                         
  if(i%4 == 0)
    {
    digitalWrite(red1,HIGH); digitalWrite(yellow1,LOW); digitalWrite(green1,LOW);
	digitalWrite(red2,HIGH); digitalWrite(yellow2,LOW); digitalWrite(green2,LOW);	
	digitalWrite(red3,HIGH); digitalWrite(yellow3,LOW); digitalWrite(green3,LOW);
	digitalWrite(red4,LOW); digitalWrite(yellow4,LOW); digitalWrite(green4,HIGH);
    delay(3000);
    digitalWrite(red1,HIGH); digitalWrite(yellow1,LOW); digitalWrite(green1,LOW);
	digitalWrite(red2,HIGH); digitalWrite(yellow2,LOW); digitalWrite(green2,LOW);
	digitalWrite(red3,HIGH); digitalWrite(yellow3,LOW); digitalWrite(green3,LOW);
	digitalWrite(red4,LOW); digitalWrite(yellow4,HIGH); digitalWrite(green4,LOW);
    delay(1000);
    }
}

}
}