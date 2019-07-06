# arduino_switch
this code is to test **switch code**

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
 pinMode(8,OUTPUT);
 pinMode(5,INPUT_PULLUP);
}

void loop() {
  // put your main code here, to run repeatedly:

 int value;

 value=digitalRead(3);

 if(value==0){
 // LED on
 digitalWrite(8,HIGH); 
 Serial.println("LED ON");
 }else{
  // LED off
  digitalWrite(8,LOW);
  Serial.println("LED OFF");
  
}
}
  
```
![arduino_switch](https://github.com/sunny9645/arduino_switch/blob/master/swith.jpg)


