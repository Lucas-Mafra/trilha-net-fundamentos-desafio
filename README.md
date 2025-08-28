# 🚗 Sistema de Estacionamento - DIO .NET Fundamentos

Projeto desenvolvido como desafio do módulo de Fundamentos da trilha .NET da [DIO](https://www.dio.me/).

## 📋 Descrição

Este sistema simula a gestão de um estacionamento, permitindo cadastrar, remover e listar veículos, além de calcular o valor cobrado pelo tempo de permanência.

## 🛠️ Funcionalidades

- **Cadastrar veículo:** Adiciona a placa de um veículo ao estacionamento.
- **Remover veículo:** Remove um veículo, solicita o tempo de permanência e calcula o valor a ser pago.
- **Listar veículos:** Exibe todos os veículos atualmente estacionados.
- **Menu interativo:** Interface simples via console para navegação entre as opções.

## 🏗️ Estrutura da Classe

A classe principal é `Estacionamento`, conforme o diagrama abaixo:

![Diagrama de classe estacionamento](diagrama_classe_estacionamento.png)

### Propriedades

- `precoInicial` (`decimal`): Preço fixo cobrado ao estacionar.
- `precoPorHora` (`decimal`): Preço cobrado por hora adicional.
- `veiculos` (`List<string>`): Lista de placas dos veículos estacionados.

### Métodos

- `AdicionarVeiculo()`: Adiciona uma placa à lista de veículos.
- `RemoverVeiculo()`: Remove uma placa, solicita as horas e calcula o valor.
- `ListarVeiculos()`: Lista todas as placas estacionadas.

## 💻 Como Executar

1. **Pré-requisitos:**  
   - [.NET 6.0 SDK ou superior](https://dotnet.microsoft.com/download)

2. **Clone o repositório:**
   ```bash
   git clone https://github.com/seu-usuario/seu-repositorio.git
   cd trilha-net-fundamentos-desafio
   ```

3. **Rode o projeto:**
   ```bash
   dotnet run
   ```

4. **Siga o menu interativo no console.**

## 📝 Exemplo de Uso

```
1 - Cadastrar veículo
2 - Remover veículo
3 - Listar veículos
4 - Encerrar

Opção: 1
Digite a placa do veículo para estacionar:
> ABC-1234
Veículo cadastrado com sucesso!

Opção: 3
Veículos estacionados:
ABC-1234

Opção: 2
Digite a placa do veículo para remover:
> ABC-1234
Digite a quantidade de horas que o veículo permaneceu estacionado:
> 2
O valor total a ser pago é: R$ 12,00
Veículo removido com sucesso!
```

## ❗ Observações

- Caso não haja veículos estacionados, será exibida a mensagem:  
  `Não há veículos estacionados.`
- O sistema não valida o formato da placa.

## 📚 Aprendizados

- Manipulação de listas e strings em C#
- Estruturas de decisão e repetição
- Interação com o usuário via console
- Encapsulamento e organização de código orientado a objetos

---

Desafio prático do curso [DIO .NET Fundamentos](https://www.dio.me/).
