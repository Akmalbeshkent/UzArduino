// UzArduino.h - Arduino kutubxonasi o'zbek tilida
#pragma once
#ifndef UZ_ARDUINO_H
#define UZ_ARDUINO_H
//#define CHIQISH         OUTPUT
//#define KIRISH          INPUT

/* ===== PIN HOLATLARI ===== */
#define CHIQISH         OUTPUT
#define KIRISH          INPUT
#define YUQORI          HIGH
#define PAST            LOW
#define PULLUP          INPUT_PULLUP

/* ===== ASOSIY FUNKTSIYALAR ===== */
#define kutish          delay
#define mikroKutish     delayMicroseconds
#define raqamliYoz      digitalWrite
#define raqamliOqi      digitalRead
#define analogOqi       analogRead
#define analogYoz       analogWrite
#define pinHolati       pinMode
#define ovoz            tone
#define ovozToxtat      noTone
#define ketmaKet        Serial

/* ===== KETMA-KET PORT ===== */
#define ketmaKetOch     Serial.begin
#define ketmaKetYoz     Serial.print
#define ketmaKetYozln   Serial.println
#define ketmaKetOqi     Serial.read
#define ketmaKetMavjud  Serial.available
#define ketmaKetToza    Serial.flush
#define ketmaKetTugat   Serial.end

/* ===== MATEMATIK AMALLAR ===== */
#define qoshish         +
#define ayirish         -
#define kopaytirish     *
#define bolish          /
#define qoldiq          %
#define ortacha         average
#define tasodifiy       random
#define tasodifiySeed   randomSeed
#define absolyut        abs
#define daraja          pow
#define ildiz           sqrt
#define yaxlit          round

/* ===== SHART OPERATORLARI ===== */
#define agar            if
#define aksHolda        else
#define uchun           for
#define va              &&
#define yoki            ||
#define emas            !
#define qaytar          return
#define davom           continue
#define toxta           break
#define almashtir       switch
#define holat           case
#define standart        default

/* ===== MA'LUMOT TURLARI ===== */
#define butun           int
#define satr            String
#define mantiqiy        bool
#define haqiqiy         float
#define doimiy          const
#define harf            char
#define uzun            long
#define qisqa           short
#define ishora          signed
#define ishorasiz       unsigned
#define massiv          array

/* ===== EEPROM ===== */
#define eepromOqi       EEPROM.read
#define eepromYoz       EEPROM.write
#define eepromYangila   EEPROM.update
#define eepromUzunOqi   EEPROM.get
#define eepromUzunYoz   EEPROM.put

/* ===== QO'SHIMCHA FUNKTSIYALAR ===== */
#define ishgaTushir     attachInterrupt
#define toxtatInterrupt detachInterrupt
#define vaqt            millis
#define mikroVaqt       micros
#define bitniOqi        bitRead
#define bitniYoz        bitWrite
#define bitniAlmashtir  bitToggle
#define baytniOqi       lowByte
#define sozniOqi        highByte

#endif // UZ_ARDUINO_H
