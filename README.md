#include "LedControl.h"
LedControl lc=LedControl(11,12,10,1); //MoxCyPython
int T = 100;

byte M_1[8] = {   
  B10100110,
  B00000000,
  B00000000,
  B00000000,
  B00000000,
  B00000000,
  B00000000,
  B00000000
};
byte M_2[8] = {   
  B10100110,
  B10000101,
  B00000000,
  B00000000,
  B00000000,
  B00000000,
  B00000000,
  B00000000
};
byte M_3[8] = {   
  B10100110,
  B10000101,
  B10010101,
  B00000000,
  B00000000,
  B00000000,
  B00000000,
  B00000000
};
byte M_4[8] = {  
  B10100110,
  B10000101,
  B10010101,
  B10010101,
  B00000000,
  B00000000,
  B00000000,
  B00000000
};

byte M_5[8] = { 
  B10100110,
  B10000101,
  B10010101,
  B10010101,
  B10010101,
  B00000000,
  B00000000,
  B00000000
};
byte M_6[8] = {  
  B10100110,
  B10000101,
  B10010101,
  B10010101,
  B10010101,
  B01101010,
  B00000000,
  B00000000
};
byte M_7[8] = {   
  B10100110,
  B10000101,
  B10010101,
  B10010101,
  B10010101,
  B01101010,
  B01101010,
  B00000000
};
byte M_8[8] = {   
  B00101010,
  B10100110,
  B10000101,
  B10010101,
  B10010101,
  B10010101,
  B01101010,
  B01101010
};
byte M_9[8] = {   
  B01101010,
  B00101010,
  B10100110,
  B10000101,
  B10010101,
  B10010101,
  B10010101,
  B01101010
};
byte M_10[8] = {   
  B01111010,
  B01101010,
  B00101010,
  B10100110,
  B10000101,
  B10010101,
  B10010101,
  B10010101
};
byte M_11[8] = {   
  B01011001,
  B01111010,
  B01101010,
  B00101010,
  B10100110,
  B10000101,
  B10010101,
  B10010101
};
byte M_12[8] = {   
  B11010101,
  B01011001,
  B01111010,
  B01101010,
  B00101010,
  B10100110,
  B10000101,
  B10010101
};
byte M_13[8] = {   
  B10010101,
  B11010101,
  B01011001,
  B01111010,
  B01101010,
  B00101010,
  B10100110,
  B10000101
};
byte M_14[8] = {  
  B10000101,
  B10010101,
  B11010101,
  B01011001,
  B01111010,
  B01101010,
  B00101010,
  B10100110
};
byte M_15[8] = {   
  B10100110,
  B10000101,
  B10010101,
  B11010101,
  B01011001,
  B01111010,
  B01101010,
  B00101010
};
byte M_16[8] = {   // array con noveno cuadro de animacion de flecha
  B00101010,
  B10100110,
  B10000101,
  B10010101,
  B11010101,
  B01011001,
  B01111010,
  B01101010
};
byte M_17[8] = {  
  B01101010,
  B00101010,
  B10100110,
  B10000101,
  B10010101,
  B11010101,
  B01011001,
  B01111010
};
void setup() {
  lc.shutdown(0,false);  
  lc.setIntensity(0,4);   
  lc.clearDisplay(0);         
    D_1();   
    delay(T);      
    D_2();       
    delay(T);      
    D_3();       
    delay(T);    
    D_4();      
    delay(T);    
    D_5();        
    delay(T);      
    D_6();    
    delay(T);   
    D_7();       
    delay(T);    
    D_8();       
}
void loop(){
    D_9();   
    delay(T);    
    D_10();   
    delay(T);      
    D_11();       
    delay(T);      
    D_12();        
    delay(T);     
    D_13();       
    delay(T);   
    D_14();        
    delay(T);    
    D_15();        
    delay(T);     
    D_16();        
    delay(T);      
    D_17();        
    delay(T);     
}
void D_1(){     
  for (int i = 0; i < 8; i++)  
  {
    lc.setRow(0,i,M_1[i]);  
  }
}
void D_2(){     
  for (int i = 0; i < 8; i++)  
  {
    lc.setRow(0,i,M_2[i]);  
  }
}
void D_3(){     
  for (int i = 0; i < 8; i++)  
  {
    lc.setRow(0,i,M_3[i]);  
  }
}
void D_4(){     
  for (int i = 0; i < 8; i++)  
  {
    lc.setRow(0,i,M_4[i]);  
  }
}
void D_5(){     
  for (int i = 0; i < 8; i++)  
  {
    lc.setRow(0,i,M_5[i]);  
  }
}
void D_6(){     
  for (int i = 0; i < 8; i++)  
  {
    lc.setRow(0,i,M_6[i]);  
  }
}
void D_7(){     
  for (int i = 0; i < 8; i++)  
  {
    lc.setRow(0,i,M_7[i]);  
  }
}
void D_8(){     
  for (int i = 0; i < 8; i++)  
  {
    lc.setRow(0,i,M_8[i]);  
  }
}
void D_9(){     
  for (int i = 0; i < 8; i++)  
  {
    lc.setRow(0,i,M_9[i]);  
  }
}
void D_10(){     
  for (int i = 0; i < 8; i++)  
  {
    lc.setRow(0,i,M_10[i]);  
  }
}
void D_11(){     
  for (int i = 0; i < 8; i++)  
  {
    lc.setRow(0,i,M_11[i]);  
  }
}
void D_12(){     
  for (int i = 0; i < 8; i++)  
  {
    lc.setRow(0,i,M_12[i]);  
  }
}
void D_13(){     
  for (int i = 0; i < 8; i++)  
  {
    lc.setRow(0,i,M_13[i]);  
  }
}
void D_14(){     
  for (int i = 0; i < 8; i++)  
  {
    lc.setRow(0,i,M_14[i]);  
  }
}
void D_15(){     
  for (int i = 0; i < 8; i++)  
  {
    lc.setRow(0,i,M_15[i]);  
  }
}
void D_16(){     
  for (int i = 0; i < 8; i++)  
  {
    lc.setRow(0,i,M_16[i]);  
  }
}
void D_17(){     
  for (int i = 0; i < 8; i++)  
  {
    lc.setRow(0,i,M_17[i]);  
  }
}
