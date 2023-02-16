# code-of-soil-moisture-sensor-in-arduin-o-uno

//here you can modify or copy
const int sensorPin = A0; // define the analog input pin for the sensor

void setup() {
  Serial.begin(9600); // initialize serial communication at 9600 bits per second
}

void loop() {
  int sensorValue = analogRead(sensorPin); // read the value from the sensor
  Serial.print("Soil Moisture: "); // print label for the value
  Serial.println(sensorValue); // print the sensor value
  delay(1000); // wait for a second before taking another reading
}


