import java.util.Scanner;
class Theater
{
 int ch;
 void doMenu()
{
Scanner in=new Scanner(System.in);
  System.out.println("1.CinePolis");
   System.out.println("2.Pvr Ripples");
    System.out.println("3.Lepl Icon");
     System.out.println("4.Capital cinemas");
      System.out.println("5.Miraj cinemas");
       System.out.println("Enter your choice");
ch=in.nextInt();
    switch(ch)
  {
  case 1:
     System.out.println("C/O PVP SQUARE MALL,4th floor MG road");
break;
 case 2:
   System.out.println("C/O PVR CINEMAS RIPPLE MALL, 3rd floor,Ripples Mall,MAin Road, MG Road");
break;
case 3:
   System.out.println("C/O INOX LEPL ICON MALL,3rd floor,LEPL ICON,Patamata");
break;
  case 4:
   System.out.println("C/O TREND SET MALL,Benz Circle");
break;
  case 5:
    System.out.println("Nageshwara rao,punthulu road, Gandhi Nagar");
break;
default:System.out.println("invalid case");
break;
}
}

void ticketcost()
{
  if(ch==1)
   System.out.println("ticket cost is 150");
 else if(ch==2)
   System.out.println("ticket cost is 135");
 else if(ch==3)
 System.out.println("ticket cost is 185");
  else if(ch==4)
System.out.println("ticket cost is 155");
  else if(ch==5)
System.out.println("ticket cost is 165");
}
void showtimings()
{
  if(ch==1)
  System.out.println("show timings are:\n Morning show-9:00Am, Afternoon show-12:00 Noon, Evening show -4:00 pm, Night-7:00pm");
 if(ch==2)
 System.out.println("show timings are:\n Morning show-10:00Am,Afternoon show-1:00pm,Evening show-5:00pm,Night-8:00pm");
if(ch==3)
 System.out.println("show timings are:\n Morning show-8:00Am,Afternoon show-11:00Am,Evening show-3:00pm,Night-6:00pm");
if(ch==4)
 System.out.println("show timings are:\n Morning show-8:30Am,Afternoon show-11:30pm,Evening show-5:30pm,Night-8:30pm");
if(ch==5)
 System.out.println("show timings are:\n Morning show-11:00Am, Afternoon show-2:00pm,Evening show-6:00pm,Night-9:00pm");
 }

int computebill(int n )
{
  if(ch==1)
  {  
 return  n*150;
   }
  else if(ch==2)
 {
     return  n*135;
 }
  else if(ch==3)
 {
     return  n*185;
  }
 else if(ch==4)
 {
    return  n*155;
  }
  else if(ch==5)
  {
    return  n*165;
  }
else
  return 0;
 }
}

 class Td1
{
public static void main(String [] args)
{
int n;
int ch;
Scanner in=new Scanner(System.in);
Theater t=new Theater();
t.doMenu();
System.out.println("enter the no.of tickets");
n=in.nextInt();
t.ticketcost();
t.showtimings();
int bill=t.computebill(n); 
System.out.println("bill is="+bill);
}
}
