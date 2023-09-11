# Esp32 Brownout

```c++
#include "soc/soc.h"
#include "soc/rtc_cntl_reg.h"

void setup()
{
  WRITE_PERI_REG(RTC_CNTL_BROWN_OUT_REG, 0); //desactiva el detector de caida de voltaje
}

void loop()
{

}
```
