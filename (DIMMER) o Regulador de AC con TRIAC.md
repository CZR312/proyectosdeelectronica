## **(DIMMER) o Regulador de AC con TRIAC**  

Al encender el circuito, el capacitor C1 empieza a cargarse a través de R1 y el potenciómetro RV2, el potenciómetro RV2 ajusta qué tan rápido se carga el capacitor y cuando el voltaje en C1 alcanza el umbral de disparo del DIAC DB3, el DIAC conduce y libera la carga acumulada. Esta corriente de disparo pasa a través de R2 hacia la compuerta del TRIAC , activándolo y el  TRIAC permite el paso de corriente a la lámpara L1, encendiéndola parcial o totalmente según el momento del disparo. Como el AC cambia de polaridad cada medio ciclo, este proceso se repite constantemente, controlando la potencia media entregada a la carga.

RV2 (500kΩ, potenciómetro): Permite ajustar la resistencia en el circuito, lo que varía el tiempo de carga del capacitor (C1). Esto controla el ángulo de disparo del TRIAC y, por lo tanto, la potencia entregada a la carga.  
R1 (10kΩ): Limita la corriente que fluye hacia el diac (D2) y el capacitor (C1), protegiendo el circuito si el potenciómetro se coloca a cero ohms por  error y controlando el tiempo de carga del capacitor.  
R2 (100Ω): Protege el diac y el TRIAC de corrientes excesivas durante el disparo, asegurando un funcionamiento estable.  
C1 (1000pF):  Junto con las resistencias (R1 y RV2), forma un circuito RC que determina el tiempo de carga. Este tiempo define el ángulo de disparo del TRIAC, regulando así la potencia entregada a la carga.  
D2 (DIAC, DB3): El Diac asegura que el TRIAC se dispare solo cuando el voltaje en el capacitor (C1) alcance su voltaje de ruptura (generalmente alrededor de 30V). Sin el Diac, el TRIAC podría activarse demasiado pronto o demasiado tarde, lo que generaría un funcionamiento errático o incluso un cortocircuito.  
U1 (TRIAC): Es el componente principal que controla el flujo de corriente alterna hacia la carga. Se dispara al recibir la señal en la compuerta mediante el diac y conduce la corriente hasta que esta cruza por cero, permitiendo el control de potencia en la carga.  
El TRIAC es como dos SCR (Thyristors) en antiparalelo, permitiendo la conducción de corriente en ambos sentidos positivo y negativo de la onda AC.  

![Image](https://github.com/user-attachments/assets/27aaa29f-58fd-4bab-91a4-0d9d80b59f78)
<img src="https://github.com/user-attachments/assets/8be39052-6677-457a-9c32-8b2d8f84e185" width="400" />
<img src="https://github.com/user-attachments/assets/ae4c6935-ed1a-40c0-adea-21300e39345c" width="400" />
