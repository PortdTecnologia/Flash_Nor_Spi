Esta biblioteca opera com memórias Flash NOR SPI via Software SPI (bit-bang),
dependendo assim do arquivo `SW_SPI.h`.
https://github.com/PortdTecnologia/Bitbang_Protocols/blob/main/SW_SPI.h

Por trabalhar em bit-bang, pode ser utilizada em qualquer microcontrolador,
mesmo aqueles que não possuem SPI por hardware, desde que haja memória
suficiente para os buffers.

Nela estão contidas funções de:

* Leitura de parâmetros de reconhecimento do fabricante, modelo e capacidade (JEDEC).
* Funções de erase de página, setor e blocos.
* Gravação e leitura de páginas de 256 bytes.
* Gravação e leitura de setores de 512 bytes para compatibilidade com sistemas de arquivos.
* Strings de alguns fabricantes pré-programadas para print serial.

### Estruturas

`Flash_JEDEC[4]`
: Fabricante, Modelo, Capacidade em Mbit e Capacidade em MegaBytes.

`Flash_Vendor[14]`
: String literal do fabricante (para os que estiverem cadastrados).

---

Dependencias: https://github.com/PortdTecnologia/Bitbang_Protocols/blob/main/SW_SPI.h

---

Mais informações:  
https://www.youtube.com/@Gustavo_PORTD
