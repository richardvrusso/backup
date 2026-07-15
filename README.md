<style>
  table {
    border-collapse: collapse !important;
    width: 100%;
    margin-bottom: 20px;
  }
  th, td {
    border: 1px solid #224422 !important; /* Faint matrix-green lines to match the Hacker theme */
    padding: 10px !important;
  }
  /* Force all images in the first column to be exact 60x60 pixel squares */
  td:first-child img {
    width: 300px !important;
    height: 300px !important;
    object-fit: contain !important; /* Prevents the image from stretching or distorting */
    background-color: transparent;  /* Keeps it clean on the dark background */
</style>
[← Back to Main Homelab Hub](https://richardvrusso.github.io/homelab/)

# OMV Backup Server
Server running OMV for homelab backups

| Preview | Product Name | Component Specifications & Notes |
| :---: | :--- | :--- |
| ![Case](https://c1.neweggimages.com/productimage/nb1280/BYJRS2509260LSB9V50.jpg) | [Sagittarius NAS Case](https://www.newegg.com/p/2AM-05KP-00014){:target="_blank"} | 8-bay NAS Pc Case Computer Case enclosure, ATX power supply, MATX motherboard, full-height PCIe, household storage,8 Hot-Swap HDD Bays PC case |
| ![Motherboard](https://www.asrockrack.com/photo/D1541D4U-2T8R-1(L).jpg) | [ASRock Rack D1541D4U-2T8R with Intel Xeon D1541 Server Processor](https://www.asrockrack.com/general/productdetail.asp?Model=D1541D4U-2T8R#Specifications){:target="_blank"} | Mini-ITX motherboard with an onboard 8-Core/16-Thread SoC CPU (45W TDP)<br>• *Features dual 10G Base-T ports and an integrated LSI 3008 HBA controller for direct drive expansion* |
| ![RAM](https://m.media-amazon.com/images/I/61o-uQu2phL._AC_SL1250_.jpg) | [SK hynix Hynix 32GB DDR4-2400 ECC RDIMM](https://a.co/d/00xAqxPr){:target="_blank"} | 2400MHz high-density registered error-correcting memory module<br>• *128GB of ECC Memory* |
| ![NVMe SSD](https://m.media-amazon.com/images/I/61tEpX718ML._AC_SL1000_.jpg) | [BPX 240GB NVMe](https://a.co/d/0bDVI8Bs){:target="_blank"} | PCIe Generation 3.0 NVMe solid state drive in M.2 2280 form factor<br>• *OS drive for OMV* |
| ![HBA Card](https://m.media-amazon.com/images/I/61BdepqlBbL._AC_SL1000_.jpg) | [LSI SAS9220-8i HBA](https://a.co/d/0ivik6cW){:target="_blank"} | Low-profile PCIe storage expansion controller card<br>• *Passes individual mechanical storage disks straight through to OpenMediaVault for native software array management* |
| ![Hard Drive](https://m.media-amazon.com/images/I/61jA7E3suuL._AC_SL1430_.jpg) | [Seagate Hard Drive](https://a.co/d/027bs6Cz){:target="_blank"} | High-capacity internal enterprise/NAS mechanical storage drive<br>• *4 drives in a mergerfs array plus one for parity* |
| ![SAS Cable](https://m.media-amazon.com/images/I/61Vx-DwuK1L._SL1000_.jpg) | [Mini SAS to 4 SATA Cable](https://a.co/d/0dgciGEh){:target="_blank"} | Internal Mini-SAS (SFF-8643) host to 4x SATA target breakout cable<br>• *Connects the onboard LSI 9220-8i controller directly to individual SATA storage drives* |
| ![Arctic Fan](https://m.media-amazon.com/images/I/61Ir6tCra7L._SL1000_.jpg) | [ARCTIC P12 PWM PST - PC Fan](https://a.co/d/09G1W2nP){:target="_blank"} | 120mm pressure-optimized case fan with PWM Sharing Technology (PST)<br>• *1 fan on the motherboard side. 2 fans on the hard drive side.* |
| ![Flex PSU](https://m.media-amazon.com/images/I/61DDEtKythL._AC_SL1000_.jpg) | [Flex ATX PSU](https://a.co/d/06jy3LsE){:target="_blank"} | Ultra-compact small form-factor (SFF) power supply unit<br>• *Provides efficient power delivery for dense server chassis, mounting perfectly via the ATX conversion bracket* |
| ![PSU Bracket](https://m.media-amazon.com/images/I/61SJVcwJnUL._AC_SL1500_.jpg) | [ATX to Flex PSU Adapter](https://a.co/d/0cM5rbtb){:target="_blank"} | Steel mounting conversion bracket adapter<br>• *Adapts a standard ATX power supply bay to securely house a compact Flex ATX form-factor PSU* |
| ![Power Adapter](https://m.media-amazon.com/images/I/61nnsCkf5ML._SL1500_.jpg) | [SATA to 4 Pin Power Cable Adapter](https://a.co/d/05aqMGHD){:target="_blank"} | SATA 15-pin male to Molex 4-pin female power connector cable<br>• *Connects PSU to hard drive backplane* |
| ![Thermal Paste](https://m.media-amazon.com/images/I/7166oBCV+PL._AC_SL1500_.jpg) | [Noctua NT-H1 3.5g, Pro-Grade Thermal Compound Paste](https://a.co/d/04wap5aV){:target="_blank"} | Premium-grade hybrid thermal interface material<br>• *Ensures optimal heat transfer from the processor lid to the heatsink with long-term stability* |
