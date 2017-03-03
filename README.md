# Zika_Algorithms
Following CDC Algorthms to export proper result of ELISA

Zika CDC ELISA

If ('P/N'<2,"Negative",If (Background<2,"Inconclusive - repeat test",If ('P/N'>=3,"Presumptive Positive","Equivocal-send for rRT-PCR")))

Zika CDC InBios ELSIA

If (ZikaISR>=1.8,"Presumptive Zika Positive",If (ZikaISR<1.8 and ZikaISR>1.6,"Re-test in Duplicate",If (ZikaAgNCA>=1.7,If (CCANCA>=1.7,"Possible Zika Positive D/D","Possible Zika Positive D/N"),If (CCANCA>=1.7,"Presumptive Other Flavivirus Positive","Negative"))))

Zika CDC InBios ELISA Repeat Condition

If (ZikaISR>=1.7,"Presumptive Zika Positive",If (ZikaAgNCA>=1.7,If (CCANCA>=1.7,"Possible Zika Positive D/D","Possible Zika Positive D/N"),If (CCANCA>=1.7,"Presumptive Other Flavivirus Positive","Negative")))
