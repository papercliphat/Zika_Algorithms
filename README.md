# Zika_Algorithms

Zika Algorithms to automate ELISA data analysis for CDC Emergency Use Authorization and InBios kit protocols. To be used with Versamax spectrophotometer.

The following links and statement are valid as of May 2017. InBios will likely improve their kit over the coming quarters and the links may change.

CDC EUA protocol is traditionally more specific than InBios with fewer false positives.

InBios protocols and documentation including EUA:
http://www.inbios.com/zikv-detecttm-igm-capture-elisa-kit-usa/

Zika CDC EUA ELISA protocol:
https://www.cdc.gov/zika/pdfs/non-eua-zika-mac-elisa-protocol.pdf

Zika CDC ELISA

If ('P/N'<2,"Negative",If (Background<2,"Inconclusive - repeat test",If ('P/N'>=3,"Presumptive Positive","Equivocal-send for rRT-PCR")))

Zika CDC InBios ELSIA

If (ZikaISR>=1.8,"Presumptive Zika Positive",If (ZikaISR<1.8 and ZikaISR>1.6,"Re-test in Duplicate",If (ZikaAgNCA>=1.7,If (CCANCA>=1.7,"Possible Zika Positive D/D","Possible Zika Positive D/N"),If (CCANCA>=1.7,"Presumptive Other Flavivirus Positive","Negative"))))

Zika CDC InBios ELISA Repeat Condition

If (ZikaISR>=1.7,"Presumptive Zika Positive",If (ZikaAgNCA>=1.7,If (CCANCA>=1.7,"Possible Zika Positive D/D","Possible Zika Positive D/N"),If (CCANCA>=1.7,"Presumptive Other Flavivirus Positive","Negative")))
