# Esp32 Brownout

```c++
#include "soc/soc.h"
#include "soc/rtc_cntl_reg.h"

void setup()
{
  WRITE_PERI_REG(RTC_CNTL_BROWN_OUT_REG, 0); //desactiva el detector de caida de voltaje y 1 para activarlo 
}

void loop()
{
}
```

Esta destinado principalmente a impedir operaciones que podrian causar daños si ocurrieran con un voltaje demasiado bajo por esta razon no es recomendado desactivarlo cuando saltan advertencias de Brownout(bajo voltaje) las causas principales son que al Esp32 no esta llegando el voltaje necesario para funcionar se debe a los cables o a la fuente de alimentacion que no puede suministrar suficiente energia
