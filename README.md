<img width="1911" height="905" alt="image" src="https://github.com/user-attachments/assets/1b969e11-e22f-47a8-9a16-0abc2f15892c" />

# **Sistema de Reservas de Hotel em OutSystems**

## **1. Introdução**
O projeto **Bookings** foi desenvolvido na plataforma **OutSystems** e tem como objetivo gerenciar reservas de quartos de hotel, com funcionalidades para:
- Visualizar e gerenciar detalhes de reservas.
- Atribuir e editar amenidades aos quartos.
- Realizar o checkout de hóspedes.
- Manter o controle de status de reservas.

## **2. Funcionalidades Principais**

### **2.1 Tela de BookingDetail**
A tela **BookingDetail** exibe detalhes de uma reserva específica, incluindo informações como:
- **Número do Quarto**: Exibe o número do quarto associado à reserva.
- **Data de Check-in e Check-out**: Permite visualizar e editar as datas de entrada e saída.
- **Status da Reserva**: Indica o estado atual da reserva (confirmada, cancelada, em andamento, etc.).

### **2.2 Tela de Bookings**
A tela **Bookings** oferece uma visão geral das reservas, com opções para:
- **Filtrar por Data**: Permite visualizar reservas por data de check-in e check-out.
- **Acessar Detalhes de Reservas**: Clicando em uma reserva específica, o usuário é direcionado à tela **BookingDetail** para editar ou visualizar os detalhes completos.

### **2.3 Tela de BookingCheckout**
A tela **BookingCheckout** permite o checkout de hóspedes, com as seguintes funcionalidades:
- **Exibição de Serviços Adicionais**: Lista de serviços de quarto consumidos durante a estadia, incluindo itens de **RoomService**.
- **Resumo de Pagamento**: Exibe o total a ser pago, incluindo serviços adicionais e taxas.
- **Confirmar Checkout**: Permite finalizar o processo de checkout e mudar o status da reserva para "concluída".

### **2.4 Lógica de Amenidades**
O sistema permite associar **RoomAmenities** aos quartos, garantindo que as reservas incluam os serviços corretos. A lógica de associação funciona da seguinte maneira:
- **Cadastro de Amenidades**: Cada quarto pode ter uma lista de amenidades associadas.
- **Exibição no BookingDetail**: As amenidades do quarto são visualizadas quando o usuário acessa os detalhes de uma reserva.

### **2.5 Gerenciamento de Status**
O sistema permite alterar o status das reservas com ações como:
- **Check-in**: Alteração do status da reserva para "em andamento".
- **Check-out**: Alteração do status da reserva para "concluída".
- **Cancelamento**: Permite cancelar a reserva, alterando o status para "cancelada".

## **3. Arquitetura do Sistema**
A arquitetura do sistema é baseada em **Agregados e Ações** para manipulação dos dados e exibição nas telas. Os principais componentes incluem:
- **Agregados de Reservas**: Manipulam dados de reservas como check-in, check-out, status e amenidades associadas.
- **Ações para Alteração de Status**: Responsáveis pela alteração do estado da reserva, como check-in, check-out e cancelamento.

## **4. Como Testar**

### **Importação dos Arquivos**
- Baixe os arquivos **BookingsCore_FM.oml** e **Bookings_FM.oml** e faça o upload na plataforma **OutSystems**.

### **Configuração do Banco de Dados**
- Certifique-se de que as tabelas de **RoomAmenities**, **Bookings**, **RoomService** e outras dependências estejam configuradas corretamente.

### **Testando Funcionalidades**
- Acesse a tela **Bookings** e crie uma nova reserva.
- Vá até **BookingDetail** para alterar os detalhes da reserva.
- Teste o checkout em **BookingCheckout**, adicionando serviços de quarto.

## **5. Conclusão**
Este projeto fornece um sistema completo de gerenciamento de reservas de hotel, com funcionalidades essenciais para a operação diária de um hotel. Ele inclui desde a criação de reservas até o checkout, além da capacidade de gerenciar amenidades e serviços de quarto.

Agora, você pode começar a usar e testar o sistema conforme os passos descritos. Para mais informações ou contribuições, entre em contato!

---

### **Links para Download dos Arquivos**
- **[BookingsCore_FM.oml](sandbox:/mnt/data/bookings_project_files/BookingsCore_FM.oml)**
- **[Bookings_FM.oml](sandbox:/mnt/data/bookings_project_files/Bookings_FM.oml)**


