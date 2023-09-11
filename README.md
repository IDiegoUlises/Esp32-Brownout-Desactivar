# Esp32 Brownout

```c++
#include "soc/soc.h"
#include "soc/rtc_cntl_reg.h"

void setup()
{
  WRITE_PERI_REG(RTC_CNTL_BROWN_OUT_REG, 0); //desactiva el detector de caida de voltaje y dar el valor de 1 en caso de activarlo 
}

void loop()
{
}
```

Esta destinado principalmente a inhibir operaciones que podrían causar daños si ocurrieran con un voltaje demasiado bajo
