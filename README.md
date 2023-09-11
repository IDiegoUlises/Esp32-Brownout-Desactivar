# Esp32 Brownout

#include "soc/soc.h"
#include "soc/rtc_cntl_reg.h"

investigar para que sirve utilizar esta libreria y para que sirve para desactivar el detector de voltaje del esp32

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
