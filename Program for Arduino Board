// C++ code

#include <Servo.h>

Servo servo_2;

void setup()
{
  pinMode(A0, INPUT);
  pinMode(9, OUTPUT);
  pinMode(10, OUTPUT);
  pinMode(11, OUTPUT);
  pinMode(0, INPUT);
  servo_2.attach(2, 500, 2500);

  pinMode(1, OUTPUT);
  pinMode(12, INPUT);
  pinMode(6, OUTPUT);
  pinMode(13, INPUT);
  pinMode(A1, INPUT);
  pinMode(3, OUTPUT);
  pinMode(2, OUTPUT);
}

void loop()
{
  if (analogRead(A0) < 330) {
    analogWrite(9, 255);
    analogWrite(10, 0);
    analogWrite(11, 0);
    if (digitalRead(0) < HIGH) {
      servo_2.write(180);
      delay(4000); // Wait for 4000 millisecond(s)
      servo_2.write(0);
      delay(4000); // Wait for 4000 millisecond(s)
      digitalWrite(1, HIGH);
      delay(10000); // Wait for 10000 millisecond(s)
      digitalWrite(1, LOW);
    }
    if (digitalRead(12) < HIGH) {
      digitalWrite(6, HIGH);
      delay(5000); // Wait for 5000 millisecond(s)
      digitalWrite(6, LOW);
    }
    if (digitalRead(13) < HIGH) {
      if (analogRead(A1) < 330) {
        digitalWrite(3, HIGH);
        delay(4000); // Wait for 4000 millisecond(s)
        digitalWrite(3, LOW);
      } else {
        if (analogRead(A1) > 330 && analogRead(A1) < 660) {
          digitalWrite(3, HIGH);
          delay(8000); // Wait for 8000 millisecond(s)
          digitalWrite(3, LOW);
        } else {
          if (analogRead(A1) > 660) {
            digitalWrite(3, HIGH);
            delay(12000); // Wait for 12000 millisecond(s)
            digitalWrite(3, LOW);
          }
        }
      }
    }
  } else {
    if (analogRead(A0) > 330 && analogRead(A0) < 660) {
      analogWrite(9, 0);
      analogWrite(10, 255);
      analogWrite(11, 0);
      if (digitalRead(0) < HIGH) {
        servo_2.write(180);
        delay(8000); // Wait for 8000 millisecond(s)
        servo_2.write(0);
        delay(8000); // Wait for 8000 millisecond(s)
        digitalWrite(1, HIGH);
        delay(10000); // Wait for 10000 millisecond(s)
        digitalWrite(1, LOW);
      }
      if (digitalRead(12) < HIGH) {
        digitalWrite(6, HIGH);
        delay(5000); // Wait for 5000 millisecond(s)
        digitalWrite(6, LOW);
      }
      if (digitalRead(13) < HIGH) {
        if (analogRead(A1) < 330) {
          digitalWrite(3, HIGH);
          delay(4000); // Wait for 4000 millisecond(s)
          digitalWrite(3, LOW);
        } else {
          if (analogRead(A1) > 330 && analogRead(A1) < 660) {
            digitalWrite(3, HIGH);
            delay(8000); // Wait for 8000 millisecond(s)
            digitalWrite(3, LOW);
          } else {
            if (analogRead(A1) > 660) {
              digitalWrite(3, HIGH);
              delay(12000); // Wait for 12000 millisecond(s)
              digitalWrite(3, LOW);
            }
          }
        }
      }
    } else {
      if (analogRead(A0) > 660 && analogRead(A0) < 1000) {
        analogWrite(9, 0);
        analogWrite(10, 0);
        analogWrite(11, 255);
        if (digitalRead(0) < HIGH) {
          servo_2.write(180);
          delay(12000); // Wait for 12000 millisecond(s)
          servo_2.write(0);
          delay(12000); // Wait for 12000 millisecond(s)
          digitalWrite(1, HIGH);
          delay(10000); // Wait for 10000 millisecond(s)
          digitalWrite(1, LOW);
        }
        if (digitalRead(12) < HIGH) {
          digitalWrite(6, HIGH);
          delay(5000); // Wait for 5000 millisecond(s)
          digitalWrite(6, LOW);
        }
        if (digitalRead(13) < HIGH) {
          if (analogRead(A1) < 330) {
            digitalWrite(3, HIGH);
            delay(4000); // Wait for 4000 millisecond(s)
            digitalWrite(3, LOW);
          } else {
            if (analogRead(A1) > 330 && analogRead(A1) < 660) {
              digitalWrite(3, HIGH);
              delay(8000); // Wait for 8000 millisecond(s)
              digitalWrite(3, LOW);
            } else {
              if (analogRead(A1) > 660) {
                digitalWrite(3, HIGH);
                delay(12000); // Wait for 12000 millisecond(s)
                digitalWrite(3, LOW);
              }
            }
          }
        }
      } else {
        digitalWrite(6, LOW);
        digitalWrite(3, LOW);
        digitalWrite(2, LOW);
        digitalWrite(1, LOW);
      }
    }
  }
}
