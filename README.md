# placa_PCI_semaforo
placa_PCI_semaforo

Desenvolvi uma placa de circuito impresso passiva para um semáforo de LEDs no KiCad. A motivação foi me familiarizar com o software, percorrendo todo o fluxo de projeto: desenho do esquemático, associação de footprints, roteamento das trilhas e verificação final no visualizador 3D.

No esquemático, atribuí cores distintas aos condutores de sinal (vermelho, amarelo e verde) para deixar imediatamente claro qual trilha alimenta cada LED — uma escolha simples que facilita muito a leitura e a revisão do circuito. Cada LED recebeu um resistor limitador dimensionado individualmente (330 Ω, 300 Ω e 220 Ω), respeitando as diferenças de tensão direta entre as cores.
<img width="722" height="507" alt="image" src="https://github.com/user-attachments/assets/5f3a6456-8dc2-46a8-b146-0379e377e2c7" />
No layout, posicionei os componentes de modo a manter os caminhos de corrente curtos e diretos, reduzindo o comprimento total de cobre e evitando desvios desnecessários — tanto por economia de material quanto por boa prática de roteamento. Também incluí quatro furos de fixação nos cantos e um retorno de GND compartilhado entre os três ramos, além de um conector de 4 vias para os sinais de controle e referência.
<img width="993" height="761" alt="image" src="https://github.com/user-attachments/assets/acd924ad-195d-40f9-9131-288f8ed80c40" />
Foi uma experiência bastante produtiva: aprendi o fluxo esquemático → PCB, o uso de PWR_FLAG e as verificações de ERC/DRC. O próximo passo é evoluir para placas com mais componentes e roteamento em duas faces.

