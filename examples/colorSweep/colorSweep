#include <EasyNeoPixels.h>

int pixelPin = 3;
int numPixels = 16;
int timer = 30;

int green[3] = {0, 255, 0};

void setup() {
  setupEasyNeoPixels(pixelPin, numPixels);
}

void loop() {
  for (int i = 0; i < numPixels; i++) {
    writeEasyNeoPixel(i, green);
    //delay(timer);
    writeEasyNeoPixel(i + 1, green);
    //delay(timer);
    writeEasyNeoPixel(i + 2, green);
    delay(timer);
    writeEasyNeoPixel(i, 0, 0, 0);
    delay(timer*2);
  }

  for (int j = numPixels; j > 0; j--) {
    writeEasyNeoPixel(j, green);
    //delay(timer);
    writeEasyNeoPixel(j - 1, green);
    //delay(timer);
    writeEasyNeoPixel(j - 2, green);
    delay(timer);
    writeEasyNeoPixel(j, 0, 0, 0);
    delay(timer*2);
  }
}
