# Sistema de Gerenciamento de Veículos

Este projeto é um simples sistema de gerenciamento de veículos desenvolvido em **Java**, utilizando conceitos de **orientação a objetos**, como **herança, encapsulamento e métodos abstratos**.

---

## Estrutura do Projeto

### Classes

- **Veiculo (abstract)**
    - Atributos:
        - `marca` (público)
        - `modelo` (público)
        - `ano` (privado)
    - Métodos:
        - `getAno()` e `setAno(int ano)`
        - `informacoesVeiculo()` (método abstrato)

- **Carro** (extends `Veiculo`)
    - Atributos adicionais:
        - `numeroPortas` (público)
    - Implementa `informacoesVeiculo()` para retornar informações completas do carro.

- **Moto** (extends `Veiculo`)
    - Atributos adicionais:
        - `cilindrada` (privado)
    - Implementa `informacoesVeiculo()` para retornar informações completas da moto.

- **Main**
    - Instancia objetos `Carro` e `Moto`
    - Define valores dos atributos
    - Exibe informações dos veículos usando o método `informacoesVeiculo()`

---

## Como Executar

1. Clone ou baixe o repositório.
2. Abra o projeto em uma IDE Java (IntelliJ, Eclipse, VSCode, etc.).
3. Compile e execute a classe `Main`.
4. Você verá a saída com as informações do carro e da moto no console:

Carro: Toyota Corolla, Ano: 2022, Portas: 4
Moto: Honda CB500, Ano: 2021, Cilindrada: 500cc


---

## Conceitos de OOP utilizados

- **Herança:** `Carro` e `Moto` herdam da classe abstrata `Veiculo`.
- **Abstração:** `Veiculo` define um método abstrato `informacoesVeiculo()` que deve ser implementado nas subclasses.
- **Encapsulamento:** atributos `ano` e `cilindrada` são privados, acessados via getters e setters.
- **Polimorfismo:** o método `informacoesVeiculo()` é implementado de forma diferente em cada subclasse.

---

## Autor

- Ricardo Henrique Coco
