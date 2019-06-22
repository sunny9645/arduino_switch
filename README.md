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
![arduino_switch](https://github.com/sunny9645/arduino_LED/blob/master/image/%EC%95%84%EB%91%90%EC%9D%B4%EB%85%B8%20%EC%8A%A4%EC%9C%84%EC%B9%98.jpg)


