XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
X                                                                           X
X                                                                           X
X   Company: Texas Instruments Norway                  X
X   Address: Gaustadalleen 21    0349 OSLO              X
X                                                                           X
X                                                                           X
X                                                                           X
XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX

PCB NAME : CC2531 USB Dongle
REVISION: 2.4
DATE: 26.01.2010

******************************************************************************
FILE: CC2531_USB_Dongle_2_4.zip 

See AN043 for information about the performance of the PCB antenna.

Design Log:
2.0 First official released version. 
2.1 Changed routing of power to pin 27, 28 and 29 to improve decoupling and meet ETSI requirement on 4.8spurius emission in RX. 
2.2 Changed discrete balun to Johanson to further reduce radiated 4.8GHz spurious when in RX, this made R251 and C251 obsolete hence removed 
      Several minor layout changes were needed to accommodate the new balun. 
2.3 Changed layout to reduce radiated VCO (4.8GHz) during RX to increase margin for ETSI requirement (-47dBm) 
      Added filter on RESET_N to reduce probability of false reset initiated by noise.
2.4 Changed Layout to reduce VCO leackage in RX, added inductor on RBIAS, removed 32kHz crystal

PCB DESCRIPTION:4 LAYER PCB 1.0 MM
      Copper        1   35 um
      Dielectric  1-2   0.25 mm (e.g. 2x Prepreg 7628 AT05 47% Resin)
      Copper        2   18 um
      Dielectric  2-3   0.50 mm (4 x 7628M 43% Resin)
      Copper        3   18 um
      Dielectric  3-4   0.25 mm (e.g. 2x Prepreg 7628 AT05 47% Resin)
      Copper        4   35 um
  DE104iML or equivalent substrate (Resin contents around 45%, which gives Er=4.42@2.4GHz, TanD=0.016)
  Dimensions in mil (0.001 inch)
  DOUBLE SIDE SOLDER MASK,
  DOUBLE SIDE SILKSCREEN,
  8 MIL MIN TRACE WIDTH AND 5 MIL MIN ISOLATION.

                 
FILE NAME                       DESCRIPTION                             FILE TYPE
-------------------------------------------------------------------------------------------
README.TXT                  THIS FILE                                   ASCII

***PCB MANUFACTURING FILES:
L1.SPL                      LAYER 1 COMPONENT SIDE/POSITIV              EXT. GERBER
L2.SPL                      LAYER 2 SOLDER SIDE/POSITIV                 EXT. GERBER
L3.SPL                      LAYER 3 COMPONENT SIDE/POSITIV              EXT. GERBER
L4.SPL                      LAYER 4 SOLDER SIDE/POSITIV                 EXT. GERBER
ASSYCOMP.SPL                ASSEMBLY DRAWING COMPONENT SIDE             EXT. GERBER
ASSYSOLD.SPL                ASSEMBLY DRAWING SOLDER SIDE                EXT. GERBER
STOPCOMP.SPL                SOLDER MASK COMPONENT SIDE/NEGATIVE         EXT. GERBER
STOPSOLD.SPL                SOLDER MASK SOLDER SIDE/NEGATIVE            EXT. GERBER
SILKCOMP.SPL                SILKSCREEN COMPONENT SIDE/POSITIVE          EXT. GERBER
SILKSOLD.SPL                SILKSCREEN SOLDER SIDE/POSITIVE             EXT. GERBER
PASTCOMP.SPL                SOLDER PAST COMPONENT SIDE/POSITIVE         EXT. GERBER
PASTSOLD.SPL                SOLDER PAST SOLDER SIDE/POSITIVE            EXT. GERBER
NCDRILL.SPL                 NC DRILL THROUGH HOLE                       EXCELLON
NCDRILL.REP                 NC DRILL REPORT                             ASCII
DRILL.SPL                   DRILL/MECHANICAL DRAWING                    EXT. GERBER
DRILL.REP                   DRILL REPORT                                ASCII
EXT_GERBER.USR              EXTENDED GERBER APERTURE TABLE              ASCII
CNC.USR                     NC DRILL DEVICE FILE                        ASCII           

***PCB ASSEMBLY FILES:

               
END.
