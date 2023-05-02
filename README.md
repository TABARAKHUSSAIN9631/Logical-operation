# Logical Operation

## AIM:

To Perform logical operation using Arduino UNO Controller.

## Software required:

Arduino IDE </br>
Proteous 

## PROCEDURE:
### Arduino IDE
Step1:Open the Arduino IDE </br>
Step2: Go to file and select new file option</br>
Step3:Type the program</br>
Step4:Go to file and select save option to save the program</br>
Step5:Go to sketch and select verify or compile options</br>
Step6:If no error Hex file will be generated in the temporary folder</br>
### Proteus 
Step7:Open the Proteus software</br>
Step8:Go to file select new design and click ok button</br>
Step9:Select component mode and click pick devices from the library</br>
Step10:Type the component name in the keyword to select the components and click ok button</br>
Step11:Design the circuit as per the diagram</br>
Step12:Double click the Arduino controller and upload the hex file generated by Arduino IDE</br>
Step13:Click start button and check the output</br>
## THEORY:
Logic gates are the basic building blocks of any digital system. It is an electronic circuit having one or more than one input and only one output. The relationship between the input and the output is based on a certain logic. Based on this, logic gates are named as AND gate, OR gate, NOT gate etc.

![image](https://user-images.githubusercontent.com/71547910/235332137-a4a37a0e-ddfb-4ca2-82e5-b1565d969413.png)

![image](https://user-images.githubusercontent.com/71547910/235332175-5d9df189-c964-45d1-ad24-e0afe6ff7eea.png)

![image](https://user-images.githubusercontent.com/71547910/235332188-bff0b03e-1b6a-4de6-993b-20497c247f17.png)

![image](https://user-images.githubusercontent.com/71547910/235332203-6bc16144-762e-40e8-ad6d-f76833a7fca4.png)

![image](https://user-images.githubusercontent.com/71547910/235332217-f598b1fb-78b6-497e-9e0e-ee2bb4dbeb71.png)

![image](https://user-images.githubusercontent.com/71547910/235332241-dd9ce66a-0e77-44d9-a699-09bfbd1968ea.png)

![image](https://user-images.githubusercontent.com/71547910/235332254-db13d222-1246-4b57-bbb2-3ab2287ccaa8.png)

## PROGRAM:
void setup() 
{</br>
pinMode(13, OUTPUT);</br>
Serial.begin(9600);</br>
}</br>
void loop() 
{</br>
if (Serial.available() > 0) {</br>
int state = Serial.read();</br>
if (state == '5') {</br>
digitalWrite(13, HIGH);</br>
Serial.println("LED ON");</br>
}</br>
if (state == '8' ) {</br>
digitalWrite(13, LOW);</br>
Serial.println("LED OFF");</br>
}</br>
}</br>
delay(50);</br>
}</br>
void setup() {</br>
Serial.begin(9600);</br>
}</br>
void loop() {</br>
Serial.print('H');</br>
delay(1000);</br>
Serial.print('L');</br>
delay(1000);</br>
}</br>

## CIRCUIT DIAGRAM:
![WhatsApp Image 2023-05-02 at 9 07 45 AM](https://user-images.githubusercontent.com/132323440/235718618-ce99d2b9-90be-4124-8bfc-7724a595f7b7.jpeg)


## OUTPUT:
![WhatsApp Image 2023-05-02 at 8 45 42 AM (1)](https://user-images.githubusercontent.com/132323440/235719965-f8931d37-6611-420b-bcc0-ecff645d25e8.jpeg)

## RESULT:
Thus the distance of the obstacle is measured using ultrasonic sensor and display the value
in serial monitor using Arduino UNO controller.
Thus the logical operation was performed by Arduino UNO controller
