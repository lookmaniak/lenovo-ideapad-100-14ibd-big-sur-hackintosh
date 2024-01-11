System Hardware,
<ul>
  <li><b>CPU: </b>Intel Core i5 5005u (Broadwell) 2.0 GHz</li>
  <li><b>GPU: </b>Intel® HD Graphics 5500</li>
  <li><b>USB: </b>2.0 and 3.0</li>
  <li><b>Memory: </b>8GB DDR3L 1600 MHz Single</li>
  <li><b>Storage: </b>SSD 250GB</li>
  <li><b>Wifi Card: </b>Broadcom BCM43xx</li>
  <li><b>Audio: </b>Conexant HD Audio CX20751/CX20752</li>
</ul>


Known Issues,
<ul>
  <li>NVDIA Discrete Graphic, not working. [disabled]</li>
  <li>Combojack Audio, external microphone not working. [internal only]</li>
  <li>Can't wake from Sleep on Battery.</li>
  <li>OEM Wifi Card doesnt work. This configuration is using BCM43xx compatible kexts (AirportBrcmFixup.kext, 
    BrcmBluetoothInjector.kext, BrcmFirmwareData.kext, BrcmPatchRAM3.kext)
    Wifi card with no Bluetooth. So, you need to adjust Kexts folder and config.plist based on your wifi card.
</li>
  <li>If your battery is dead, SMCBatteryManager.kext will cause Kernel Panic. 
    To fix this, replace the battery or Remove SMCBatteryManager.kext from kext and config.plist. 
    </li>
  <li>Dead battery can also causing Trackpad in System Preference not working, however mouse emulation and
    gestures is still working.</li>
  <li>Card reader is not tested, probably not working.</li>
  <li>-- what I'm not mentioned here, is working fine.</li>
</ul>
