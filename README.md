# Servo Motor Interfacing 

##  AIM:
To control the speed and direction of servomotor using Arduino UNO controller.

## Software required:
Arduino IDE </br>
Proteous

## PROCEDURE:
### Arduino IDE
Step1:Open the Arduino IDE </br>
Step2: Go to file and select new file option </br>
Step3:Type the program </br>
Step4:Go to file and select save option to save the program </br>
Step5:Go to sketch and select verify or compile options </br>
Step6:If no error Hex file will be generated in the temporary folder </br>
### Proteus
Step7:Open the Proteus software </br>
Step8:Go to file select new design and click ok button </br>
Step9:Select component mode and click pick devices from the library </br>
Step10:Type the component name in the keyword to select the components and click ok button </br>
Step11:Design the circuit as per the diagram </br>
Step12:Double click the Arduino controller and upload the hex file generated by Arduino IDE </br>
Step13:Click start button and check the output

## THEORY:

## PROGRAM:
#include <Servo.h></br>
Servo myservo;</br>
int pos = 0;</br>
void setup()</br>
{</br>
myservo.attach(4);</br>
}void loop()</br>
{</br>
for(pos = 0; pos <= 180; pos += 1)</br>
{</br>
myservo.write(pos);</br>
delay(15);</br>
}</br>
for(pos = 180; pos>=0; pos-=1)</br>
{</br>
myservo.write(pos);</br>
delay(15);</br>
}</br>
}</br>

## CIRCUIT DIAGRAM:
![image](https://github.com/AMANKUMAR2541/Servo-Motor-Interfacing/assets/132323363/da716c99-9b71-4e3d-9bb6-21bff688f2b8)


## OUTPUT:
![image](https://github.com/AMANKUMAR2541/Servo-Motor-Interfacing/assets/132323363/6a8328cf-647e-4af8-80db-d0ebca6fe0da)


## RESULT:
Thus the speed and direction of the servomotor was controlled using Arduino UNO controller.
