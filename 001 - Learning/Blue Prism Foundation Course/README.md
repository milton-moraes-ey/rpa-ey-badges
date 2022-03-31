## 001 - Introdução

### **O que é RPA?**

- Automação de tarefas repetitivas e com regras bem definidas, usando um software que é instalado no computador do usuário. Esse software, normalmente, é chamado de BOT;
- O BOT é programado para executar a sequencia de passos que os humanos fazem em seus processos;
- O BOT irá trabalhar da mesma maneira que um humano executa seu processo, interagindo com a interface gráfica das aplicações. Ou seja, não é integrado.

### **Quais as vantagens em usar RPA?**

- Tecnologias RPA não são invasivas, permitindo que se trabalhe com sistemas, banco de dados e estruturas TI já existentes, sem a necessidade de modificação nos mesmos;
- Bots podem trabalhar 24x7;
- Bots podem trabalhar com diferentes plataformas como Windows, Web apps, Java, entre outros;
- Um único robô pode ser programado para executar mais de um processo em diferentes horários;
- Aumenta a eficiência e acurácia.

### **Limitações do RPA**

- A velocidade de execução da automação é limitada a velocidade da aplicação que está sendo automatizada;
- Tarefas que necessitam de julgamentos e criatividade não podem ser automatizadas, uma vez que o RPA é recomendado para tarefas repetitivas, bem definidas e com decisões binárias (sim ou não);
- A depender do tipo de interação entre o robô e a aplicação, principalmente as interações referentes a interface gráfica, qualquer tipo de alteração na estrutura da interface, necessita que o robô seja reconfigurado.

---

## Control Room, Work Queues, Multi Bot

**Qual a importância de uma Work Queue?**

Dado uma automação em que devemos processar 10.000 itens de dados de determinada fonte de dados, por exemplo uma planilha de Excel, e que cada um desses itens leve em torno de 10 segundos para serem processados. Portanto, para processar os 10.000 dados, uma automação levaria cerca de 1.000.000 de segundos ou 28 horas. 

Em relação ao caso descrito, quais seriam as estratégias de trabalho para otimizar o tempo de processamento desses dados?

Uma dessas estratégias seria distribuir os 10.000 itens em mais bots, ou seja, em mais automações. Para que isso seja possível, devemos distribuir nossos dados no que o Blue Prism chama de Queue (fila em português).   A fila nos da a possibilidade de distribuir seus itens - dados de processamento -  em diferentes automações, fazendo com que os bots não processe os mesmos itens que já estão sendo ou irão ser processados por outra automação. Além de que, a fila, nos garante que não teremos perca de tempo de processamento, caso algum dado a ser processado chegue a falhar durante o processo de execução da automação.

Outra característica da fila, o que garante a viabilidade operacional desse recurso em ambientes de produção, é seu back-log de trabalho, em que pode-se conferir quais são os status e demais informações a respeito do processamento dos itens processados. Viabilizando a possibilidade de auditoria da fila e garantia de seu funcionamento dentro dos conformes.