# Esp32-Desactiva-Brown

#include "soc/soc.h"
#include "soc/rtc_cntl_reg.h"

investigar para que sirve utilizar esta libreria que es para desactivar el detecto de voltaje del esp32

```c++
#include "soc/soc.h"
#include "soc/rtc_cntl_reg.h"

void setup() {
  WRITE_PERI_REG(RTC_CNTL_BROWN_OUT_REG, 0); //disable   detector
  //Your code
}

void loop()
{
}
```
