# Hardware_Control_Handle_Rotation

Sistema embarcado para controle de rotação de punho em próteses bioelétricas através de sensores inerciais.

O sistema conta com a utilização de dois acelerometro acoplados ao paciente, acoplados respectivamente em paralelo na região antero-lateral do torax nos musculos intercostais e outro localizado no triceps braquial. O funcionamento está baseado na agulação criada entre os sensores pelo movimento de abdução do braço, gerando assim um movimento de pronação e supinação da protese.

O circuito eletronico conta com a utilização de um micrcontrolador STM32F103C8T6, com toda parte de Debug, reset e clock adicionada ao circuito. 

As proteses mioeletricas atuais contam na maioria das vezes com motores DC e para o acionamento do mesmo foi utilizado do driver L293D, que consegue controlar a velocidade e sentido de rotação do motor através da modulação dos pulsos de PWM gerado.

Já para a parte de entrada de dados foi definido o sensor MPU6050, contando com protocolo de comunicação I2C.
