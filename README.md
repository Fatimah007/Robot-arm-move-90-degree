# Robot-arm-move-90-degree

By using the code.

#include <Servo.h>

int i = 0;

int p = 0;

int j = 0;

Servo servo_9;

void setup()
{
  servo_9.attach(9, 500, 2500);

}

void loop()
{
  p = 0;
  for (p = 1; p <= 89; p += 1) {
    servo_9.write(p);
    delay(20); // Wait for 20 millisecond(s)
  }

  for (j = 89; j >= 1; j -= 1) {
    servo_9.write(p);
  }
}

![b25e3b6e-f5a9-421f-86d0-7460e4c8fa26](https://user-images.githubusercontent.com/86019166/126908482-85b87e91-56be-4eba-9d8b-a80669b3383a.jpg)
