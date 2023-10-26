# 3.3-Conceptos-de-UF2-ELF-BOOTLOADER-Firmware
/*
 * Nombre del Archivo: main.c
 * Autor:   Donovan Rojo Chaidez
 * Correo:  l21210424@tectijuana.edu.mx
 * Fecha:   25/oct/2023
 * Curso:   Lenguajes de Interfaz, TECNM Campus ITT
 * 
 * Objetivo:
 * Este programa está diseñado para que imprima la tabla de sumar hasta 12 + 12
 *
 * Historial de Revisiones:
 * 25/Oct/2023        Donovan Rojo Chaidez - Creado
 *
 */

#include <stdio.h>
#include "pico/stdlib.h"

int main() {
  stdio_init_all();

  for (int i = 1; i <= 12; i++) {
    for (int j = 1; j <= 12; j++) {
      int suma = i + j;
      printf("%d + %d = %d\n", i, j, suma);
    }
  }

  while (true) {
    sleep_ms(250);
  }
}
