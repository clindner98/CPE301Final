# CPE301Final
CPE301 Final project 

void setup() {
  
   float Fahrenheit;

}

void loop() {
  // put your main code here, to run repeatedly:

}

//Function to read temperature sensor
void getTemp(){

  sensorValue = analogRead(sensorPin); //reads sensor
  
  Fahrenheit = sensorValue; //convert to Fahrenheit

  return Fahrenheit;  //Function will output Fahrenheit
}

//Function to compare Fahreinheit to threshold
void compareToThreshold(getTemp){

  int threshold = 50; //Arbitrary constant set as threshold
  bool FanOnOff;  //Output to go next function
  
  if (getTemp>threshold){ // if-else to compare threshold to temp and set output variable
    FanOnOff = 1;
  }
  else if(getTemp<threshold){
    FanOnOff = 0;
  } 

  return FanOnOff; 
}

//Function to turn fan on/off based on comparison to threshold
void Fan(compareToThreshold){

}
