Sewage Flow Rate Measurer
Published on 22.11.2016
Written on 23.06.2016 by Luke Cockerton, University of Cambridge
Team Members:
Samad Arshad (mechanical),
Sarah Wong (electrical),
Luke Cockerton (software)

Background:
The Cambridge Development Initiative is a student-run organisation that operate in Tanzania to empower the community. The engineering team are solving WASH problems by addressing sanitation issues. They are piloting (2016) a sanitation model where sewage is transported away from homes via simplified sewerage. The innovation is that this waste is then processed in an anaerobic biogas digester which extracts methane. However there is a problem of blockage in the biogas digester, which is believed to be due to sediment/sands/soil coming in from unprotected seals in the simplified sewerage network. A way to address this is to create a settling tank that separates sewage from sediment. But to create a settling tank, one needs to know the volumetric flowrate of the sewage. There is no current method to measure the volumetric flow-rate of sewage - only a guesstimate is used. A concept of a tipping bucket was thought of to measure a mass flow-rate of sewage. The sewage flow-rate measurer is a single bucket which receives in waste from the top, and tips over because of the shift in centre of mass as the bucket fills with sewage. The pros is that its simple to construct in Tanzania, with simple electronics and software. The cons is that the bucket is susceptible to clogging up with solids which affects its tipping ability. 

Code description:
This code was written to suppliment the hardware for the Sewage-flowrate-measurer device.
use logging_code.txt in an Arduino script. 

Hardware:
  pinMode(13,OUTPUT); // Cleaning LED
  This LED signals that the bucket needs to be cleaned/go under maintainence. This is detected because of unusually large delay time between tipped bucket and restored bucket.

  pinMode(12,OUTPUT); // Use pin 12 as the lower LED
  This LED signals that the bucket is in its 'tipping' position. Used for debugging purposes.

  pinMode(11,OUTPUT); // Use pin 11 as the upper LED 
  This LED signals that the bucket is in its 'upright' position. Used for debugging purposes.
