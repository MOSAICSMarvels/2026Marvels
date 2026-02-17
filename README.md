# 2026Marvels
#include <kipr/wombat.h>

int main()
{
    printf("Hello World\n");
    
    cmpc(3);
   
   motor(0,-100);
    motor(3,-98);
    msleep(1000);
    
ao();
msleep(500);
    
    cmpc(3);
    
    while (gmpc(3) < 2400)
{
 motor(0,0);
 motor(3,98);
}
ao();
msleep(500);
    
    cmpc(3);
    
    motor(0,97);
    motor(3,100);
    msleep(2500);
    
    while (analog (0) <= 1500)
    {
    if (analog (0) <= 1500)
        { 
            motor(0,100);
            motor(3,98);
        }
        
        
    }
    cmpc(3);
    
    motor(0,-97);
    motor(3,-100);
    msleep(100);
    
    ao();
    msleep(500);
    
    cmpc(3);
    
    while (gmpc(3) < 2400)
{
 motor(0,0);
 motor(3,98);
}
ao();
msleep(500);
    
    
 while(analog (5) <= 3700)
    {
    if (analog (0) <= 1300)
        { 
            motor(0,20);
            motor(3,100);
        }
    else if ((analog (0) >= 1301)) 
          { 
            motor(0,100);
            motor(3,20);
          }
             else 
             {
                 motor(0,100);
                 motor(3,100);
             }
    }
    
    return 0;
}

