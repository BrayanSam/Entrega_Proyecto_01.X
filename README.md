Entrega_Proyecto_01.X
/*
 * File:   LED_avr-main.c
 * Author: Solis Hernandez Brayan Samuel 
 * Grupo: 7CV7
 * Created on 23 de abril de 2021, 02:46 PM
 */
#define F_CPU 1000000UL
#include <xc.h>
#include <stdint.h>
#include <util/delay.h>



int main(void) {
    DDRB=0xFF;
    while (1) 
    {
    PORTB = 0x01;	
    _delay_ms(250);                                             
    PORTB = 0x00;    
    }
}
