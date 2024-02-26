# SETA-CARRO

// código C++ // const int buttonPinE = 9; const int buttonPinD = 10; const int buttonPin2 = 11; int buttonStateE = 0; int buttonStateD = 0; int buttonState2 = 0;

void setup() { pinMode(buttonPinE,INPUT); pinMode(botãoPinD,INPUT); pinMode(botãoPin2,INPUT); pinMode(13, OUTPUT);//SETA ESQUERDA pinMode(12, OUTPUT);//SETA ESQUERDA pinMode(11, OUTPUT);//SETA DIREITA pinMode(10, OUTPUT);//SETA DIREITA

}

loop vazio() {

buttonStateE = digitalRead(buttonPinE); buttonStateD = digitalRead(buttonPinD); buttonState2 = digitalRead(botãoPin2);

//esquerda if (buttonStateE ==HIGH){

digitalWrite(1,ALTO); digitalWrite(2, ALTO);

atraso(1000);

digitalWrite(1, BAIXO); digitalWrite(2, BAIXO);

atraso(1000);

} outro {

digitalWrite(1,BAIXO); digitalWrite(2, BAIXO);

}

//direita if (buttonStateD == HIGH){

digitalWrite(3,ALTO); digitalWrite(4, ALTO);

atraso(1000);

digitalWrite(3, BAIXO); digitalWrite(4, BAIXO);

atraso(1000);

} outro {

digitalWrite(3,BAIXO); digitalWrite(4, BAIXO);

}

//pisca alerta if (buttonState2 == HIGH){

digitalWrite(3,ALTO); digitalWrite(4,ALTO); digitalWrite(1,ALTO); digitalWrite(2,ALTO);

atraso(1000);

digitalWrite(3, BAIXO); digitalWrite(4, BAIXO); digitalWrite(1,BAIXO); digitalWrite(2, BAIXO);

atraso(1000);

} outro {

digitalWrite(3,BAIXO); digitalWrite(4, BAIXO);

} }
