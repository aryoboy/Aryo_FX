
_________________________________________
==================================
/*---------PARABOLIC SAR---------------*/
/*---------------------------------------*/ 
//check sar diatas atau dibawah
//jika sar di atas maka hasilnya  = 2
//jika sar di bawah maka hasilnya = 1 
/*---------------------------------------*/ 
int QnSAR(int shift=0){
   int result=0;
   double pSAR = iSAR(NULL,0,0.02,0.2,shift);

   if(pSAR<=Low[shift]) result = 1;
   if(pSAR>=High[shift]) result = 2;
return(result);}
