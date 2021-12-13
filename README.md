# Adagio-system
This project is a first attempt to create automatic data collection system for water flow readings 
This work was developed as a course project of a student of the Perm Aviation Technical School on the specialty of a radio operator (7 semester out of 8)

This project include four parts of the system: 
    - Information collection client (ICC) - this element collect, packeting and sending all data, which was was received;
    - Client unit (CU) - this element accumulates the number of revolutions of the water flow meter shaft;
    - Data warehouse server (DWS) - this element store all information, which was received from ICC by Ethernet-communication;
    - Data visualization client (DVC) - this element this element makes a request to the server to receive data for a certain period, visualizes them, and export is also       possible. In other words, this is a custom application;
    
 This work was an educational project with an innovative proposal for the optimization of human labor in an enterprise.
 Disadvantages of this project:
      ICC:  - Shift register the 74HC165 gives out incorrect information. 74HC165 need the output and input hardware filter;
     (hard.)- ENC28J60 in the first prototype was not placed on the printed circuit board, instead, like the main controller, it was fixed with a wall-mounted solderless               mounting using shields;
            - Was not checked cuting of a signal from the CU;
            - Status register need the input hardware filter;
      ICC:  - Shift register the 74HC165 gives out incorrect information. A placeholder line has been added in the ICC code (see the link @correct_str_1);
            -
            
            
