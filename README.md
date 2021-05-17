# Line-Following-Robot
#include <mega16.h>
#define s1 PINA.0
#define s2 PINA.1
#define s3 PINA.2
#define s4 PINA.3
#define s5 PINA.4

void main()
{
DDRC=0xff;
PORTC=0x00;
DDRA=0x00;                
DDRB.3=0;
PORTB.3=1;
while (1)
{
if (s1==0&&s2==0&&s3==1&&s4==0&&s5==0)
{
PORTC.0=1;
PORTC.1=0;
PORTC.6=1;
PORTC.7=0;
DDRB.3=1;
OCR0 = 0x25; //to generate 20% duty cycle
TCCR0 = 0x69; //Configure fast PWM, non-inverted, without prescaler
}
if (s1==0&&s2==1&&s3==0&&s4==0&&s5==0)
{
PORTC.0=1;
PORTC.1=0;
PORTC.6=1;
PORTC.7=0;
DDRB.3=1;
OCR0 = 0x25; //to generate 20% duty cycle
TCCR0 = 0x69; //Configure fast PWM, non-inverted, without prescaler
}if (s1==0&&s2==0&&s3==0&&s4==1&&s5==0)
{
PORTC.0=1;
PORTC.1=0;
PORTC.6=1;
PORTC.7=0;
DDRB.3=1;
OCR0 = 0x25; //to generate 20% duty cycle
TCCR0 = 0x69; //Configure fast PWM, non-inverted, without prescaler
}if (s1==0&&s2==1&&s3==0&&s4==1&&s5==0)
{
PORTC.0=1;
PORTC.1=0;
PORTC.6=1;
PORTC.7=0;
DDRB.3=1;
OCR0 = 0x25; //to generate 20% duty cycle
TCCR0 = 0x69; //Configure fast PWM, non-inverted, without prescaler
}
if (s1==0&&s2==0&&s3==1&&s4==1&&s5==0)
{
PORTC.0=1;
PORTC.1=0;
PORTC.6=1;
PORTC.7=0;
DDRB.3=1;
OCR0 = 0x25; //to generate 20% duty cycle
TCCR0 = 0x69; //Configure fast PWM, non-inverted, without prescaler
}
if (s1==0&&s2==1&&s3==1&&s4==0&&s5==0)
{
PORTC.0=1;
PORTC.1=0;
PORTC.6=1;
PORTC.7=0;
DDRB.3=1;
OCR0 = 0x25; //to generate 20% duty cycle
TCCR0 = 0x69; //Configure fast PWM, non-inverted, without prescaler
}
if (s1==0&&s2==1&&s3==1&&s4==1&&s5==0)
{
PORTC.0=1;
PORTC.1=0;
PORTC.6=1;
PORTC.7=0;
DDRB.3=1;
OCR0 = 0x25; //to generate 20% duty cycle
TCCR0 = 0x69; //Configure fast PWM, non-inverted, without prescaler
}
if (s3==0&&s4==0&&s2==0&&s5==0&&s1==1)
{
PORTC.0=1;
PORTC.1=0;
PORTC.6=0;
PORTC.7=0;
DDRB.3=1;
OCR0 = 0x10; //to generate 20% duty cycle
TCCR0 = 0x69; //Configure fast PWM, non-inverted, without prescaler
}
if (s1==1&&s2==1&&s3==1&&s4==1&&s5==0)
{
PORTC.0=1;
PORTC.1=0;
PORTC.6=0;
PORTC.7=0;
DDRB.3=1;
OCR0 = 0x10; //to generate 20% duty cycle
TCCR0 = 0x69; //Configure fast PWM, non-inverted, without prescaler
}
if (s1==1&&s2==1&&s3==0&&s4==0&&s5==0)
{
PORTC.0=1;
PORTC.1=0;
PORTC.6=0;
PORTC.7=0;
DDRB.3=1;
OCR0 = 0x10; //to generate 20% duty cycle
TCCR0 = 0x69; //Configure fast PWM, non-inverted, without prescaler
}
if(s1==0&&s2==0&&s3==1&&s4==1&&s5==1)
{
PORTC.0=0;
PORTC.1=0;
PORTC.6=1;
PORTC.7=0;
DDRB.3=1;
OCR0 = 0x10; //to generate 20% duty cycle
TCCR0 = 0x69; //Configure fast PWM, non-inverted, without prescaler
}
if(s1==0&&s2==0&&s3==0&&s4==1&&s5==1)
{
PORTC.0=0;
PORTC.1=0;
PORTC.6=1;
PORTC.7=0;
DDRB.3=1;
OCR0 = 0x10; //to generate 20% duty cycle
TCCR0 = 0x69; //Configure fast PWM, non-inverted, without prescaler
}
if(s1==0&&s2==0&&s3==0&&s4==0&&s5==1)
{
PORTC.0=0;
PORTC.1=0;
PORTC.6=1;
PORTC.7=0;
DDRB.3=1;
OCR0 = 0x10; //to generate 20% duty cycle
TCCR0 = 0x69; //Configure fast PWM, non-inverted, without prescaler
}
if(s1==0&&s2==1&&s3==1&&s4==1&&s5==1)
{
PORTC.0=0;
PORTC.1=0;
PORTC.6=1;
PORTC.7=0;
DDRB.3=1;
OCR0 = 0x10; //to generate 20% duty cycle
TCCR0 = 0x69; //Configure fast PWM, non-inverted, without prescaler
}
}
}
