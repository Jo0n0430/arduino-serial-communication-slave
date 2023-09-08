# arduino-serial-communication-slave
Arduino serial communication between Leonardo and Uno(slave)
#include <SoftwareSerial.h>
SoftwareSerial mySerial(A1,A0);

void setup(){
   mySerial.begin(9600); //아두이노간 통신
   Serial.begin(9600);  // 컴퓨터, 아두이노간 통신

}

void loop(){
   if(mySerial.available(){
     char data = mySerial.read();
     Serial.print(data);
}
