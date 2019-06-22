# arduino_switch
arduino **switch**

## parts list

* arduino
* switch
* wire
* bread board


## arduino code

```cpp
void setup() {
  // put your setup code here, to run once:
 Serial.begin(9600);
 pinMode(13,OUTPUT);
 pinMode(3,INPUT_PULLUP);
}

void loop() {
  // put your main code here, to run repeatedly:

 int value;

 value=digitalRead(3);

 if(value==0){
 // LED on
 digitalWrite(13,HIGH); 
 Serial.println("LED ON");
 }else{
  // LED off
  digitalWrite(13,LOW);
  Serial.println("LED OFF");
  
}
}
  
```


